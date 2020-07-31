//HTML
<div class="container">
  <p id="count">0</p>
</div>
<div class="btns">
  <button id="down" onclick="countDown();">Subtract1</button>
  <button id="up" onclick="countUp();">Add 1</button>
</div>

body{
  background:#344;
}

---------

//CSS
.container{
  height:200px;
  width:600px;
  background:#fff;
  margin:0 auto;
  border: 3px solid gold;
}
.container p{
  text-align:center;
  padding-top:50px;
  font-size:38px;
  border:0;
  width:100%;
}
.btns{
  margin:0 auto;
  width:600px;
  text-align:center;
  margin-top:10px;
}
button{
  width:100px;
  height:50px;
  margin:0px 5px;
  border-radius:3px 3px 3px;
  border:none;
  background:#c04;
  color:#fff;
  font-size:16px;
}

--------

//JS
button:hover{
  cursor:pointer;
}
button:focus{
  outline:none;
}

function countUp(){
  var total = parseInt(document.getElementById("count").value, 10);
  total = isNaN(total) ? 0 : total;
  total ++;
  document.getElementById('count').value = total;
  document.getElementById('count').innerHTML = total;
}
function countDown(){
  var total = parseInt(document.getElementById("count").value, 10);
  total = isNaN(total) ? 0 : total;
  total --;
  document.getElementById('count').value = total;
  document.getElementById('count').innerHTML = total;
}
