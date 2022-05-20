### _Experience Tabs_ project

> _Tabs with conditional css and varied data_ project

![](public/tabs.gif)

<!-- > Live demo [_here_](https://www.example.com). If you have the project hosted somewhere, include the link here. -->

<!-- <hr style="border:1px dotted lightblue"> </hr> -->

#### General Information

Purpose of the project is to train myself on:

- using useState, loading true/false logic
- useEffect and data fetching
- applying conditional class properties

#### Technologies Used

- React.Js

#### Code Elements

- Changing state value -> and displaying corresponding data from the list
- Adding css value ('active-btn' class) based on certain condition

```javascript
const { company, dates, duties, title } = jobs[value];
    ...
    ...
    ...
{jobs.map((item, index) => {
  // index - represents placement in the array
  return (
    <button
      key={item.id}
      onClick={() => setValue(index)}
      className={`job-btn ${index === value && 'active-btn'}`}
    >
      {item.company}
    </button>
   );
})}

```

#### Installation and project setup

After you clone this repo to your desktop, go to its root directory and run `npm install` to install its dependencies.

Once the dependencies are installed, you can run `npm start` to start the application. You will then be able to access it at `localhost:3000`

##### Acknowledgements

Credits to an awesome instructor John Smilga!
