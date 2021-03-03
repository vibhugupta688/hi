# final-project-demo-2


In Index.html :
   <div>
      <button  id = "btn" type="button" class="btn btn-primary btn-lg">Timer</button>
    </div>
    <div>
      <button  id = "stBtn" type="button" class="btn btn-primary btn-lg">Stop Timer</button>
    </div>
    
    
 
 
 In Script.js:
 
 
const stopNum = document.querySelector("h1");
const btn = document.querySelector("#btn")
const Stopbtn = document.querySelector("#stBtn")
let num = 10;
let timeRef

const timer = () =>{
  stopNum.innerHTML ="Loading...."

 timeRef  =  setInterval( ()=>{
  stopNum.innerHTML = `${num}`;
  num--
  },1000)
   console.log(timeRef);
}

btn.addEventListener("click",timer)

Stopbtn.addEventListener("click", ()=>{
clearInterval(timeRef)
})
       
