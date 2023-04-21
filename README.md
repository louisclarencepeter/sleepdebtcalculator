# Sleep Tracker

This is a simple program that helps you keep track of how much sleep you're getting each week and lets you know if you're getting enough sleep or not.

## Getting Started

To use the program, simply download or clone the repository and run the `index.js` file. You can run the program by typing `node index.js` in your terminal or command prompt.

## Usage

The program will prompt you to enter the number of hours of sleep you got for each day of the week, starting with Monday. Once you've entered all the hours, the program will tell you the total number of hours of sleep you got that week, as well as whether you got enough sleep or not.

## How it works

The program uses the following formula to calculate your ideal sleep hours for the week:

```
idealSleepHours = 8 * 7;
```

This assumes that you should aim to get 8 hours of sleep per night and that there are 7 days in a week.

The program then asks you to enter the number of hours of sleep you got for each day of the week and calculates the total number of hours using the following function:

```
function getActualSleepHours() {
  const weekSleepHours =
    getSleepHours("monday") +
    getSleepHours("tuesday") +
    getSleepHours("wednesday") +
    getSleepHours("thursday") +
    getSleepHours("friday") +
    getSleepHours("saturday") +
    getSleepHours("sunday");

  return weekSleepHours;
}
```

The `getSleepHours()` function takes a day of the week as an argument and returns the number of hours of sleep you got on that day. The `getActualSleepHours()` function calls this function for each day of the week and adds up the total number of hours.

The program then compares the actual number of hours of sleep you got to your ideal number of sleep hours using the following code:

```
if (actualSleepHours === idealSleepHours) {
  console.log("You got the perfect amount of sleep this week!");
} else if (actualSleepHours > idealSleepHours) {
  console.log("You got more sleep than you needed this week.");
} else {
  console.log(
    "You got " +
      (idealSleepHours - actualSleepHours) +
      " hour(s) less sleep than you needed this week. Get some rest!"
  );
}
```

If you got the perfect amount of sleep, the program will tell you so. If you got more sleep than you needed, the program will let you know. And if you got less sleep than you needed, the program will tell you how many hours you need to make up.

## Contributing

If you find any bugs or have any suggestions for how to improve the program, feel free to create a pull request or submit an issue on the repository. I welcome contributions from anyone who wants to help make the program better!

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
