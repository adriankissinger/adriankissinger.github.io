const wordsTeam1 = [];
const wordsTeam2 = [];

document.addEventListener('keydown', keyPressed);

let b = 0;
function addWord(){
	var e = document.getElementById("1");
	var input = document.getElementById("input");
	if (e.checked == 1) {
		wordsTeam1.push(input.value);
	} else {
		wordsTeam2.push(input.value);
	}
	input.value = "";
}

function keyPressed(e){
	if (e.code == 'Enter'){
		addWord();	
	}
}

function nextWord(){
	shuffle(wordsTeam1);
	shuffle(wordsTeam2);
	var x = document.getElementById("lblOutput");
	if (b == 0){
		x.innerHTML = wordsTeam1[0];
		wordsTeam1.splice(0, 1);
		b = 1;
	} else {
		x.innerHTML = wordsTeam2[0];	
		wordsTeam2.splice(0, 1);
		b = 0;
	}
}


function shuffle(a) {
    var j, x, i;
    for (i = a.length - 1; i > 0; i--) {
        j = Math.floor(Math.random() * (i + 1));
        x = a[i];
        a[i] = a[j];
        a[j] = x;
    }
    return a;
}