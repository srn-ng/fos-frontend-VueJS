
<template>
  <section>
    <div class="container">
      <div class="contactInfo">
        <div>
        <h2>Contact info</h2>
        <ul class="Info">
          <li>
            <img src="/images/location.png" alt="" class="imgC">
            <span>137 ter Bd Colonel Krim Belkacem, Algiers</span>
          </li>
          <li>
            <img src="/images/mail.png" alt="" class="imgC">
            <span>contact@finishoffschool.com</span>
          </li>
          <li>
            <img src="/images/call.png" alt="" class="imgC">
            <span>05555555555</span>
          </li>
        </ul>
       </div> 
      </div>
      <div class="contactForm">
        <h2>Contactez-nous</h2>
        <div class="formBox">
          <div class="inputBox w50">
            <input type="text" required >
            <span>Votre nom</span>
            
          </div>
          <div class="inputBox w50">
            <input type="text" required >
            <span>Adresse Email</span>
            
          </div>
          <div class="inputBox w50">
            <input type="text"  required >
            <span>Numéro de téléphone</span> 
            
          </div>
          <div class="inputBox w100">
            <textarea name="" required></textarea>
            <span>Ecrivez votre message ici...</span>
            
          </div>
          <div>
            <button class="button-contact">Envoyer</button>
          </div>
        </div>
      </div> 
    </div>
  
  </section>
  
</template>

<style>



*
{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Poppins' , sans-serif;
}
section{
    margin-top:200px ;
    position: relative;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    display: flex;
    background-color: rgb(255, 255, 255);
 }
 section::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 45%;
  height: 100%;
  background-color:rgb(255, 255, 255) ;
  
} 

.container{
  padding: 0;
  margin: 0;
  position: relative;
  width: 700px;
  min-height: 500px;
  z-index: 1000;
  display: flex;
  
  
}

.container .contactInfo{
  position: absolute;
  top: 50px;
  width: 250px;
  height: calc(100% - 90px);
  background-color:#046380 ;
  color: white;
  z-index: 1;
  padding: 10% 0;
  display: flex;
  /* justify-content: center; */
  align-items: center;
  flex-direction: column;
  justify-content: space-between;
  box-shadow: 0 18px 22px rgba(0, 0, 0, 0.15);
}
.container .contactInfo  ul.Info{
  position: relative;
  margin: 20px 0px;
  color: white;

}
.container .contactInfo  ul.Info li{
  position: relative;
  list-style: none;
  display: flex;
  margin: 25px 0;
  cursor: pointer;
  align-items: flex-start;
  color: white;
}
.container .contactInfo  ul.Info li span:nth-child(1) {
  width: 25px;
  min-width: 25px ;
  color: white;
}
.container .contactInfo  ul.Info li span:nth-child(1) img {
  max-width: 100%;
  filter: invert(1);
}
.container .contactInfo  ul.Info li span:nth-child(2) {
  color: white;
  margin-left:10px ;
  font-size: 80%;

}
.container .contactInfo h2
{
  color: white;
  font-size: 20px;
  display: flex;
  white-space: nowrap;
  justify-content: center;
}



.imgC{
  width: 14%;
  height: 14%;
}


.container .contactForm{
  position: absolute;
  padding: 40px 40px;
  padding-left: 200px;
  margin-left: 150px;
  width: calc(100% - 150px);
  color: rgb(83, 82, 82);
  height: 100%;
  background-color: rgb(219, 218, 218);
  box-shadow: 0 50px 50px rgba(0, 0,0, 0.25);

}
.container .contactForm h2 {
  color: #046380;
  font-size: 30px;
  white-space: nowrap;
  display: flex;
  margin-left:0% ;
}
.container .contactForm .formBox{
  position: relative;
  display: flex;
  justify-content: space-between;
  flex-direction: column;
  white-space: nowrap;
  /* padding-top:1% ; */
  font-size:14px ;
}
.container .contactForm .formBox .inputBox{
  position: relative;
  margin-bottom: 13%;
}
.container .contactForm .formBox .inputBox.w50{
  width: 35%;
}
.container .contactForm .formBox .inputBox.w100{
  width: 100%;
}
.inputBox input {
  border-bottom: 1px solid rgb(131, 131, 131);
  width: 250px;
 
  font-size: 19px;
  outline: none;
  
  /* border-radius: 8% ; */
}
.inputBox textarea {

  border-bottom: 0.01px solid rgb(131, 131, 131);
  width: 250px;
  outline: none;
}
.button-contact{
  background: #046380;
  margin-left:55% ;
  margin-top:4% ;
  padding: 5px;
  width: 30%;
  border-radius:15% ; 
  font: 600;
  color: #ffffff;
  font-size:100%;
}
.button-contact:hover{
  background: #0393be;
}
.container .contactForm .formBox .inputBox span{
  position: absolute;
  left: 0;
  padding: 5px 0;
  pointer-events: none;
  transition: 0.3s;
}
.container .contactForm .formBox .inputBox input:focus ~ span ,
.container .contactForm .formBox .inputBox input:valid ~ span ,
.container .contactForm .formBox .inputBox textarea:focus ~ span ,
.container .contactForm .formBox .inputBox textarea:valid ~ span 
{
  transform: translateY(-20px);
  font-size: 11px;
  color: #115d74;
  font-weight: 400;

}

  

</style>







