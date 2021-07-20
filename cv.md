# Denis Shneidar 
![It is me](https://avatars3.githubusercontent.com/u/48366912?s=460&v=4 "My Photo")

### *Contact Info:* 
* Phone Number +375-44-732-94-96 
* *[Email](https://anrowerdd@gmail.com)*
* *[VK](https://vk.com/id114568964)*
* *[Telegram](https://t.me/Anrower)*

### *Summary*:

* #### *About:*
    The most important thing for me it's not wasting time,
    constantly studing, learn something new. My goal's 
    is to become a front-end developer. I can focus on a task. I react correctly to criticism and draw conclusions from it.
* #### *Goals:*
    * Hard Skills:
        1. [x] HTML basic knowlege;
        2. [x] CSS basic knowlege;
        3. [+-] JS core;
        4. [x] GIT basic;
        5. [ ] OOP fundamentals;
        6. [+-] Experience with Node.js and npm
        7. [ ] Experience with Vue.js, React JS, Angular or TypeScript;
        8. [+-] CSS preprocessor (SCSS/LESS/SASS) one of them;
        9. [x] English level A2 or higher;
        10. [+-] WebPack
    * Soft skills:    
        1. [ ] Teamwork
        2. [ ] Leadership
        3. [ ] Presentation
    ---

* #### *Projects*
    * [Landing Save a Life](https://save-life-anrower.netlify.app/#take-home)
    * [Todo app (js)](https://vigilant-hoover-9df2fa.netlify.app/)
    * [Momentum app (js)](https://anrower.github.io/momentum/)
    ---

* #### *Favorite quotes:*

    > ***Sanity*** -  the most effective behavior for a given set of conditions.

    > The brain does not know anything, until it gets experience


    has been ascribed to Jacque Fresco.

---
### *Skills*: 
 * Hard Skills:
    1. Html - basic knowledge
    2. CSS - basic knowledge
    3. JS - basic JS
    4. Git - basic commands
    5. English - A2

* Soft Skills:
    1. Never stop learning
    2. Communication
    3. Conclusion

---
### *Code examples:* 
```javascript
function whoseBicycle(diary1, diary2, diary3) {
  
  let firstSonSumMarks = getSumMarks(diary1),
      secondSonSumMarks = getSumMarks(diary2),
      thirdSonSumMarks = getSumMarks(diary3);
      
  const ageTable = {
    'firstSonAge': 14,
    'secondSonAge': 9,
    'thirdSonAge': 8
  }
  
  function getSumMarks(obj) {
    let sum = 0;
    for (let key in obj) {
      sum += obj[key];
    }
    return sum;
  } 

  class Son {
    
    constructor(age, sumMarks, index) {
      this.age = age,
      this.sumMarks = sumMarks,
      this.index = index;
    }

  }

  let firstSon = new Son(ageTable.firstSonAge, firstSonSumMarks, 'first'),
      secondSon = new Son(ageTable.secondSonAge, secondSonSumMarks, 'second'),
      thirdSon = new Son(ageTable.thirdSonAge, thirdSonSumMarks, 'third')
      
  let sonsArr = [firstSon, secondSon, thirdSon];

  sortByMarksValue(sonsArr);
  
  function sortByMarksValue (arr) {
    arr.sort(function (a, b) {
      if (a.sumMarks > b.sumMarks) {
        return 1;
      }
      if (a.sumMarks < b.sumMarks) {
        return -1;
      }
      return 0;
    });
  }
  
  let [a, b, c] = sonsArr;
  
  if(c.sumMarks !== b.sumMarks) {
    return `I need to buy a bicycle for my ${c.index} son.`
    
  }else if(c.sumMarks === b.sumMarks && c.sumMarks !== a.sumMarks) {
    let result = (c.age < b.age) ?
        `I need to buy a bicycle for my ${c.index} son.` :
        `I need to buy a bicycle for my ${b.index} son.`;
    return result;
    
  }else {
    let result = (c.age < b.age && c.age < a.age) ?
        `I need to buy a bicycle for my ${c.index} son.` :
        (b.age < c.age && b.age < a.age) ?
        `I need to buy a bicycle for my ${b.index} son.` :
        `I need to buy a bicycle for my ${a.index} son.`;

    return result;
  }
         
}
```
---