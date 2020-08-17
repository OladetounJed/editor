<template>
  <div class="home">
   <div class="editor">
     <div class="editor__header">
        <h1 class="editor__heading">Listbuy Editor</h1>
        <a href="#" class="editor__deploy">Live</a>
     </div>
     <div class="editor__area">
       <h1 class="editor__sub-heading">Edit Your Element</h1>
        <div class="editor__child">
          <h1 class="editor__title">Header</h1>
          <input type="text" name="" placeholder="Header Text" class="editor__input">
          <input type="text" name="" placeholder="Header Font Size" class="editor__input">
        </div>
        <div class="editor__child">
          <h1 class="editor__title">Paragraph</h1>
          <input type="text" name="" placeholder="Paragraph Text" class="editor__input">
          <input type="text" name="" placeholder="Paragraph Font Size" class="editor__input">
        </div>
        <button class="editor__submit">Submit</button>
     </div>
    
     

   </div>
   <div class="live">
     <iframe name="Framename" src="https://octavia-pay.web.app/" width="100%" height="100%" frameborder="0" scrolling="auto" class="live__area">
</iframe>
   </div>
  </div>
</template>

<script>


export default {


}
</script>
<style lang="scss">
//Fonts
$primary-font: "Open Sans";
$secondary-font: "Epilogue";

//Colors
$primary-black: #000;
$primary-white: #ffff;
$primary-smokewhite: #fafafa;
$primary-yellow: #d0c930;
$primary-grey: #716767;

$secondary-black: #212121;
$secondary-grey: #707070;
*{
  margin: 0;
  padding: 0;
  font-family: $primary-font;
}

.home {
  display: flex;
}
.editor {
  width: 50%;
  &__header {
    display: flex;
    justify-content: space-between;
    margin: 1em 2em;
  }
  &__heading {
    font-size: 1.3em;
  }

&__sub-heading {
  font-size: 2em;
  color: rgba($primary-grey, .7);
  margin: 1.5em 0;
  padding-bottom: .5em;
  border-bottom: 0.1em solid rgba($primary-black, .9);
  
}
&__title {
  margin-left: 3em;
  font-size: 1.5em;
}
  &__input {
      display: block;
      border: none;
      margin: 2em auto;
      border: 0.1em solid $secondary-grey;
      outline: none;
      height: 3em;
    background-color: transparent;
    padding-left: 1em;
    width: 50%;
    color: $primary-black;
  }
  &__submit {
    display: block;
    border: none;
     height: 4em;
    width: 15em;
    padding: 0;
    color: $primary-white;
    background-color: $primary-black;
    font-weight: 700;
    margin: 2em auto;
  }
  &__deploy {
    padding: .5em 2em;
    color: $primary-white;
    background-color: $primary-yellow;
    text-decoration: none;
  }
}

.live {
  height: 100vh;
  width: 50%;

}



</style>
