<script>
export default {
  data() {
    return {
      quizpost: [
        { id: 1, title: 'HTMLquest', body: 'Quwstion1'},
        { id: 2, title: 'HTMLquest', body: 'Quwstion2'},
        { id: 3, title: 'HTMLquest', body: 'Quwstion3'},
      ]
    }
  }
}
</script>

<template>
    <main class="app">
 <h1>The Admin panel</h1>
 <div class="quiz">
   <h3>Quiz redaction</h3>
   <form>
     <input class="input" type="text" placeholder="Text question">
     <input class="input" type="text" placeholder="Text question">
     <input class="input" type="text" placeholder="Text question">
     <button class="btn" @click="addLike">Add quiz-post</button>
   </form>
 <div class="quiz-post" v-for="post in quizpost">
       <div>Quiz HTML {{ post.title }}</div>
       <div>HTML {{ post.body }}</div>
 <input type="text">
 <textarea name="" id="" cols="30" rows="30"></textarea>
  
 <button @click="addLike">Add question {{ likes }}</button>
 <button @click="addDisLike">End question {{ dislikes }}</button>
 <button>Click me! {{ likes }}</button>
 <button>Click me! {{ dislikes }}</button>
 </div>
 <div class="quiz-post">
 <div>Quiz CSS</div>
 
 <input type="text">
 <textarea name="" id="" cols="30" rows="30"></textarea>
  
 <button @click="addLike">Dislake! {{ dislikes }}</button>
 <button @click="addDisLike">Dislakes! {{ dislikes }}</button>
 <button>Click me! {{ likes }}</button>
 <button>Click me! {{ dislikes }}</button>
 </div>
 <div class="quiz-post">
 <div>Quiz JS</div>
 
 <input type="text">
 <textarea name="" id="" cols="30" rows="30"></textarea>
  
 <button @click="addLike">Dislake! {{ dislikes }}</button>
 <button @click="addDisLike">Dislakes! {{ dislikes }}</button>
 <button>Click me! {{ likes }}</button>
 <button>Click me! {{ dislikes }}</button>
 </div>
 </div>
 
    </main>
 </template>
 
 <style>
 *{
 margin: 0;
 padding: 0;
 box-sizing: border-box;
 font-family: 'Roboto', sans-serif;
 }
 
 body {
 background-color: #e4e0eb;
 color: #FFF;
 }
 
 .app {
   display: flex;
   flex-direction: column;
   align-items: center;
   padding: 2rem;
   min-height: 100vh;
 }
 
 h1 {
    font-size: 2rem;
    margin-bottom: 2rem;
 }
 
 .quiz {
    background-color: #ac84e6;
    padding: 15px;
    width: 100%;
    max-width: 640px;
    border: 2px solid #b9f1dc;
 }
 .quiz-post {
    background-color: #ac84e6;
    padding: 15px;
    width: 100%;
    max-width: 640px;
    border: 2px solid #5e2aee;
    margin-top: 15px;
 }
 
 button {
   appearance: none;
   outline: none;
   border: 2px;
   cursor: pointer;
 padding: 2px 3px;
 background-color: #eaedf3;
 color: #422177;
  font-weight: 700;
  text-transform: uppercase;
  font-size: 14px;
  border-radius: 5px;
 }
 
 button:disabled {
  opacity: 0.5;
 }
 
 .input {
   width: 100%;
   border: 2px solid #13e7a8;
   padding: 18px 14px;
   margin-top: 14px;
 }
 
 form: {
   display: flex;
   flex-direction: column;
 }
 
 .btn {
   margin-top: 15px;
   align-self: flex-end;
   background: none;
   color: #13e7a8;
   border: 2px solid #13e7a8;
 }
 </style>
 