<template>
  <main>
    <div class="overlay">
      <div class="modal">
        <textarea name="note" id="note" cols="30" rows="10"></textarea>
        <button>Add Note</button>
        <button id="close">Close</button>
      </div>
    </div>
    <div class="container">
      <header>
        <h1>Notes</h1>
        <button>+</button>
      </header>
      <div class="cards-container">
        <div class="cards">
          <p class="main-text">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Odit quas doloremque, debitis voluptate provident ex?</p>
          <p class="date">lorem</p>
        </div>
      </div>
    </div>
  </main>
</template>

<style scoped>
main{
  height: 100vh;
  width: 100vw;
}
.overlay{
  position: absolute;
  width: 100%;
  height: 100%;
  background-color: rgba(0,0,0,0.66);
  z-index: 10;
  display: flex;
  justify-content: center;
  align-items: center;
}
.container{
  max-width: 1000px;
  padding: 10px;
  margin: 0 auto;
}
header{
  display: flex;
  justify-content: space-between;
  align-items: center;
}
h1{
  font-weight: bold;
  margin-bottom: 25px;
  font-size: 75px;
}
header button{
  border: none;
  padding: 10px;
  width: 50px;
  height: 50px;
  cursor: pointer;
  background-color: rgb(21,20,20);
  border-radius: 100%;
  color: aliceblue;
  font-size: 20px;
}
.cards-container{
  display: flex;
}
.cards{
  width: 225px;
  height: 225px;
  background-color: rgb(237,182,44);
  padding: 10px;
  border-radius: 15px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  margin-right: 20px;
  margin-bottom: 20px;
}
.date{
  font-size: 12.5px;
  font-weight: bold;
  text-align: center;
}
.modal{
  width: 750px;
  background-color: azure;
  border-radius: 10px;
  padding: 30px;
  position: relative;
  display: flex;
  flex-direction: column;
}
.modal button{
  padding: 10px 20px;
  font-size: 20px;
  width: 50%;
  margin: 25px auto 0 auto;
  background-color: #ccc;
  color: white;
  border: none;
  cursor: pointer;
  border-radius: 16px;
}
#close{
  background-color: red;
}
</style>