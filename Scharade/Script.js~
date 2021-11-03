const wordsTeam1 = [];
const wordsTeam2 = [];
let b = 0;
function addWord(){
	var x = document.getElementById("frm1");
	if (x.elements[0].checked == 1) {
		wordsTeam1.push(x.elements[2].value);
	} else {
		wordsTeam2.push(x.elements[2].value);
	}
	x.elements[2].value = "";
}

function nextWord(){
	shuffle(wordsTeam1);
	shuffle(wordsTeam2);
	var x = document.getElementById("lbl2");
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