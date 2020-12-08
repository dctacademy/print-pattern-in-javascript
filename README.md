# print-pattern-in-javascript
programs for printing pyramid patterns
```javascript
const n = 5
// Left Half-Pyramid Pattern in JavaScript
// Output
//     *
//    **
//   ***
//  ****
// *****
function createHalfPyramid (height) {
  
    for (var i = 1; i <= height; i++) {
      var row = '';
      
      for (var j = 1; j <= (height - i); j++) {
        row += ' ';
      }
      
      for (var k = 1; k <= i; k++) {
        row += '*';
      }
      
      console.log(row);
    }
  }
  createHalfPyramid(n);

// Down Side Right Half Pyramid in JavaScript
// *****
// ****
// ***
// **
// *
function downSideRightHalfPyramid(n){
    for(let i=1;i<=n;i++){
        let row = ""
        for(let j=1;j<=(n-i+1);j++){
            row += "*"
        }
        console.log(row)
    }
}
downSideRightHalfPyramid(n);


// Down Side Left Half Pyramid in JavaScript
// *****
//  ****
//   ***
//    **
//     *
function downSideLeftHalfPyramid (height) {
  
    for (var i = 1; i <= height; i++) {
      var row = '';
  
      for (var j = 1; j <= (i - 1); j++) {
        row += ' ';
      }
  
      for (var j = 1; j <= (height - i + 1); j++) {
        row += '*';
      }
          
      console.log(row);
    }
  }
  
  downSideLeftHalfPyramid(n);

// Right Half Pyramid Pattern with star in JavaScript
// *
// **
// ***
// ****
// *****
function rightHalfPyramid (height) {

    for (let i = 1; i <= height; i++) {
      let row = '';
  
      for (let j = 1; j <= i; j++) {
        row += '*';
      }
  
      console.log(row);
    }

  }
  
  rightHalfPyramid(n);

// Two Pyramid in one patterns in JavaScript
// *
// **
// ***
// ****


// ****
// ***
// **
// *
  function rightHalfTwoPyramid(height) {
    let result = ""
    for (let i = 1; i <= height; i++) {
        let row = ""
      for (let j = 1; j <= i; j++) {
        row += '*';
      }
      console.log(row);
    }
    console.log("\n");
    for (let i = height; i >= 0; i--) {
        let row = ""
      for (let j = 1; j <= i; j++) {
        row += '*';
      }
      console.log(row);
    }
  }
  rightHalfTwoPyramid(n);

// Two Pyramid in one patterns in JavaScript
// *****
// ****
// ***
// **
// *

// *
// **
// ***
// ****
// *****
function twoPyramidsInOne(height){
  for (let m = height; m >= 0; m--) {
      let s = ""
      for (let n = 1; n <= m; n++){
          s += "*"
      }
      console.log(s)
  }
  for (let m = 1; m <= height; m++) {
      let s = ""
      for (let n = 1; n <= m; n++){
          s += "*"
      }
      console.log(s);
  }
}


// Pyramid pattern in JavaScript
//     *
//    * *
//   * * *
//  * * * *
// * * * * *
function pyramid1(height){
  let a = '';
  let m = (height-1); 
  for(i=1; i <= height; i++)
  {
      a = a.trim();
      a = ' '.repeat(m) + a + (i > 1 ? ' ' : '') + '*';
      console.log(a);
      m--;
  }
}
pyramid1(n);

// Pyramid with tab space
// 				*		
// 			*		*		
// 		*		*		*		
// 	*		*		*		*		
// *		*		*		*		*
function pyramid2(height){
  let str = '';
  for(let i=1; i<=height; i++){
      for(let k=1; k<=height-i; k++){
          str += "\t";
      }
      for(let j=1; j<=i; j++){
          str += "*\t\t";
      }
      console.log(str);
      str = "";
  }
}
pyramid2(n);

// Right Side Pyramid Pattern in JavaScript
// * 
// * * 
// * * * 
// * * * * 
// * * * * * 
// * * * * * * 
// * * * * * 
// * * * * 
// * * * 
// * * 
// * 
function rightSidePyramid(height){
  const star = "* ";
  //where length is no of stars in longest streak
  const length = height;
  for(let i = 1; i <= (length*2)-1; i++){
     const k = i <= length ? i : (length*2)-i;
     console.log(star.repeat(k));
  }
}
rightSidePyramid(n);


// diamond Shape in JavaScript

//     * 
//    * * 
//   * * * 
//  * * * * 
// * * * * * 
//  * * * * 
//   * * * 
//    * * 
//     *
function creatediamondShape(size){
    for(var i=1;i<=size;i++){
       for(var s=size-1;s>=i;s--){
          process.stdout.write(" ");
       }
       for(var j=1;j<=i;j++){
          process.stdout.write("* ")
       }
       console.log();
    }
    if(i==size+1){
       for(var i=1;i<=size-1;i++){
          for(var s=1;s<=i;s++){
             process.stdout.write(" ");
          }
          for(j=i;j<=size-1;j++){
             process.stdout.write("* ");
          }
          console.log();
       }
    }
 }
 creatediamondShape(n);
 ```

