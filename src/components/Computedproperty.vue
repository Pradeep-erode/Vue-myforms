<template>
<h2>husgd</h2>
  <div class="grid"> pradeep
  </div>
  
</template>

<script>

export default {
name:'flower-rose'

}

export const exportdirectconstant = 'The Lord of the Rings Trilogy';
function greeting(a,b) {
	console.log(a + b);
}

// once defined that must be exported or used with in the methods  used in that component other it gave error mesage
// function subtract() {
// 	console.log('werwe');
// }

//we cannot use funtion outside export ,once used that must be exported like below,

const bestMovieSeriess = 'The Lord';

export  { greeting, bestMovieSeriess }

export const UiGrid  = {
  // ...
  render() {
    return (
      <div>
       i AM render from render option 
      </div>
    );
  },
};

</script>


<style>

</style>