<!-- AUTOGEN:STATS -->
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript) [![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML) [![Terminal](https://img.shields.io/badge/mac%20terminal-000000?style=for-the-badge&logo=apple&logoColor=white&labelColor=000000)](https://support.apple.com/guide/terminal/welcome/mac) [![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)](https://code.visualstudio.com/) [![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/) [![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)](https://www.figma.com/) 

[![📊 Views](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/VuToV-Mykola/goit-js-hw-05/main/assets/db/visitors-badge.json)](https://github.com/VuToV-Mykola/goit-js-hw-05/graphs/traffic)
[![⭐ Stars](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/VuToV-Mykola/goit-js-hw-05/main/assets/db/likes-badge.json)](https://github.com/VuToV-Mykola/goit-js-hw-05/actions/workflows/screenshot-and-visitor.yaml)
[![📦 Size](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/VuToV-Mykola/goit-js-hw-05/main/assets/db/repo-size.json)](https://github.com/VuToV-Mykola/goit-js-hw-05)
[![📄 License](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/VuToV-Mykola/goit-js-hw-05/main/assets/db/repo-license.json)](https://github.com/VuToV-Mykola/goit-js-hw-05/blob/main/LICENSE)

## 📸 Скріншот проекту
![Project Screenshot](./assets/screenshot.png)
<!-- END:AUTOGEN -->

## My Achievements

![Description](./assets/head.jpg)

## My Certificates - Completed Sololearn Course:

![Certification Badge](./assets/certificat.jpg)

[SOLOLEARN](https://www.sololearn.com/certificates/CT-VJXN3HQH)

# JavaScript Homework 05

## Task 1. User Names

**COMPLETE THIS TASK IN THE FILE `task-1.js`**

Write an arrow function `getUserNames(users)` that accepts one parameter `users` — an array of user objects. The function should return an array of all user names (the `name` property) from the `users` array.

Take the code below and insert it after declaring your function to check the correctness of its work. The console will display the results of its calls.

```javascript
console.log(
  getUserNames([
    {
      name: "Moore Hensley",
      email: "moorehensley@indexia.com",
      balance: 2811
    },
    {
      name: "Sharlene Bush",
      email: "sharlenebush@tubesys.com",
      balance: 3821
    },
    {
      name: "Ross Vazquez",
      email: "rossvazquez@xinware.com",
      balance: 3793
    },
    {
      name: "Elma Head",
      email: "elmahead@omatom.com",
      balance: 2278
    },
    {
      name: "Carey Barr",
      email: "careybarr@nurali.com",
      balance: 3951
    },
    {
      name: "Blackburn Dotson",
      email: "blackburndotson@furnigeer.com",
      balance: 1498
    },
    {
      name: "Sheree Anthony",
      email: "shereeanthony@kog.com",
      balance: 2764
    },
  ])
); // ["Moore Hensley", "Sharlene Bush", "Ross Vazquez", "Elma Head", "Carey Barr", "Blackburn Dotson", "Sheree Anthony"]
```

Leave this code for mentor verification.

### Mentor Review Criteria

- Declared variable `getUserNames`
- The variable `getUserNames` is assigned an arrow function with parameter `(users)`
- The `map()` method is used to iterate over the `users` parameter
- Calling the function with the specified array of users returns the array `["Moore Hensley", "Sharlene Bush", "Ross Vazquez", "Elma Head", "Carey Barr", "Blackburn Dotson", "Sheree Anthony"]`
- Calling the function with random but valid arguments returns the correct value

## Task 2. Users with Friend

**COMPLETE THIS TASK IN THE FILE `task-2.js`**

Write an arrow function `getUsersWithFriend(users, friendName)` that accepts two parameters:

- first parameter `users` — an array of user objects
- second parameter `friendName` — the name of a friend to search for

The function should return an array of all users from the `users` array who have a friend with the name `friendName`. Each user's friends are stored in the `friends` property. If there are no users with such a friend, the function should return an empty array.

**Tips:**

- The `filter()` method can be used to create a new array with elements that satisfy a certain condition
- Use the `includes()` method to check if the `friends` array contains `friendName`

Take the code below and insert it after declaring your function to check the correctness of its work. The console will display the results of its calls.

```javascript
const allUsers = [
  {
    name: "Moore Hensley",
    friends: ["Sharron Pace"]
  },
  {
    name: "Sharlene Bush",
    friends: ["Briana Decker", "Sharron Pace"]
  },
  {
    name: "Ross Vazquez",
    friends: ["Marilyn Mcintosh", "Padilla Garrison", "Naomi Buckner"]
  },
  {
    name: "Elma Head",
    friends: ["Goldie Gentry", "Aisha Tran"]
  },
  {
    name: "Carey Barr",
    friends: ["Jordan Sampson", "Eddie Strong"]
  },
  {
    name: "Blackburn Dotson",
    friends: ["Jacklyn Lucas", "Linda Chapman"]
  },
  {
    name: "Sheree Anthony",
    friends: ["Goldie Gentry", "Briana Decker"]
  }
];

console.log(getUsersWithFriend(allUsers, "Briana Decker")); 
// [
//   {
//     name: "Sharlene Bush",
//     friends: ["Briana Decker", "Sharron Pace"]
//   },
//   {
//     name: "Sheree Anthony",
//     friends: ["Goldie Gentry", "Briana Decker"]
//   }
// ]

console.log(getUsersWithFriend(allUsers, "Goldie Gentry"));
// [
//   {
//     name: "Elma Head",
//     friends: ["Goldie Gentry", "Aisha Tran"]
//   },
//   {
//     name: "Sheree Anthony",
//     friends: ["Goldie Gentry", "Briana Decker"]
//   }
// ]

console.log(getUsersWithFriend(allUsers, "Adrian Cross")); // []
```

Leave this code for mentor verification.

### Mentor Review Criteria

- Declared variable `getUsersWithFriend`
- The variable `getUsersWithFriend` is assigned an arrow function with parameters `(users, friendName)`
- The `filter()` method is used to iterate over the `users` parameter
- If the value of the `friendName` parameter is the string `"Briana Decker"`, the function returns an array of user objects with names `Sharlene Bush` and `Sheree Anthony`
- If the value of the `friendName` parameter is the string `"Goldie Gentry"`, the function returns an array of user objects with names `Elma Head` and `Sheree Anthony`
- If the value of the `friendName` parameter is the string `"Adrian Cross"`, the function returns an empty array
- Calling the function with random but valid arguments returns the correct value

## Task 3. Sorting by Number of Friends

**COMPLETE THIS TASK IN THE FILE `task-3.js`**

Write an arrow function `sortByDescendingFriendCount(users)` that accepts one parameter `users` — an array of user objects.

The function should return an array of all users sorted in descending order by the number of their friends (the `friends` property).

Take the code below and insert it after declaring your function to check the correctness of its work. The console will display the results of its calls.

```javascript
console.log(
  sortByDescendingFriendCount([
    {
      name: "Moore Hensley",
      friends: ["Sharron Pace"],
      gender: "male"
    },
    {
      name: "Sharlene Bush",
      friends: ["Briana Decker", "Sharron Pace"],
      gender: "female"
    },
    {
      name: "Ross Vazquez",
      friends: ["Marilyn Mcintosh", "Padilla Garrison", "Naomi Buckner"],
      gender: "male"
    },
    {
      name: "Elma Head",
      friends: ["Goldie Gentry", "Aisha Tran"],
      gender: "female"
    },
    {
      name: "Carey Barr",
      friends: ["Jordan Sampson", "Eddie Strong"],
      gender: "male"
    },
    {
      name: "Blackburn Dotson",
      friends: ["Jacklyn Lucas", "Linda Chapman"],
      gender: "male"
    },
    {
      name: "Sheree Anthony",
      friends: ["Goldie Gentry", "Briana Decker"],
      gender: "female"
    }
  ])
);
// [
//   {
//     name: "Ross Vazquez",
//     friends: ["Marilyn Mcintosh", "Padilla Garrison", "Naomi Buckner"],
//     gender: "male"
//   },
//   {
//     name: "Sharlene Bush",
//     friends: ["Briana Decker", "Sharron Pace"],
//     gender: "female"
//   },
//   {
//     name: "Elma Head",
//     friends: ["Goldie Gentry", "Aisha Tran"],
//     gender: "female"
//   },
//   {
//     name: "Carey Barr",
//     friends: ["Jordan Sampson", "Eddie Strong"],
//     gender: "male"
//   },
//   {
//     name: "Blackburn Dotson",
//     friends: ["Jacklyn Lucas", "Linda Chapman"],
//     gender: "male"
//   },
//   {
//     name: "Sheree Anthony",
//     friends: ["Goldie Gentry", "Briana Decker"],
//     gender: "female"
//   },
//   {
//     name: "Moore Hensley",
//     friends: ["Sharron Pace"],
//     gender: "male"
//   }
// ]
```

Leave this code for mentor verification.

### Mentor Review Criteria

- Declared variable `sortByDescendingFriendCount`
- The variable `sortByDescendingFriendCount` is assigned an arrow function with parameter `(users)`
- The `toSorted()` method is used to iterate over the `users` parameter
- Calling the function with the specified `users` array returns a new array of users sorted in descending order by the number of their friends
- Calling the function with random but valid arguments returns the correct value

## Task 4. Total Balance by Gender

**COMPLETE THIS TASK IN THE FILE `task-4.js`**

Write an arrow function `getTotalBalanceByGender(users, gender)` that accepts two parameters:

- first parameter `users` — an array of user objects
- second parameter `gender` — a string storing the gender

The function should use method chaining and return the total balance of users (the `balance` property) whose gender (the `gender` property) matches the value of the `gender` parameter.

Take the code below and insert it after declaring your function to check the correctness of its work. The console will display the results of its calls.

```javascript
const clients = [
  {
    name: "Moore Hensley",
    gender: "male",
    balance: 2811
  },
  {
    name: "Sharlene Bush",
    gender: "female",
    balance: 3821
  },
  {
    name: "Ross Vazquez",
    gender: "male",
    balance: 3793
  },
  {
    name: "Elma Head",
    gender: "female",
    balance: 2278
  },
  {
    name: "Carey Barr",
    gender: "male",
    balance: 3951
  },
  {
    name: "Blackburn Dotson",
    gender: "male",
    balance: 1498
  },
  {
    name: "Sheree Anthony",
    gender: "female",
    balance: 2764
  }
];

console.log(getTotalBalanceByGender(clients, "male")); // 12053

console.log(getTotalBalanceByGender(clients, "female")); // 8863
```

Leave this code for mentor verification.

### Mentor Review Criteria

- Declared variable `getTotalBalanceByGender`
- The variable `getTotalBalanceByGender` is assigned an arrow function with parameters `(users, gender)`
- Method chaining is used in the function body in the correct order
- The value of the `users` parameter is not modified
- If the value of the `gender` parameter is the string `"male"`, the function returns the number `12053`
- If the value of the `gender` parameter is the string `"female"`, the function returns the number `8863`
- Calling the function with random but valid arguments returns the correct value
