// getting the Number of Sleep Hours

function getSleepHours(day) {
  if (day === "monday") {
    return 7;
  } else if (day === "tuesday") {
    return 6;
  } else if (day === "wednesday") {
    return 8;
  } else if (day === "thursday") {
    return 8;
  } else if (day === "friday") {
    return 5;
  } else if (day === "saturday") {
    return 6;
  } else if (day === "sunday") {
    return 7;
  }
}

// getting the total sleep hours that you actually slept

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

// getting the ideal sleep hours that you prefer

function getIdealSleepHours() {
    const idealHours = 8;
    return idealHours * 7;
  }

// calculating the sleep debt

function calculateSleepDebt() {
    const actualSleepHours = getActualSleepHours();
    const idealSleepHours = getIdealSleepHours();
  
    if (actualSleepHours === idealSleepHours) {
      console.log("You got the perfect amount of sleep this week.");
    } else if (actualSleepHours > idealSleepHours) {
      console.log(
        "You got " +
          (actualSleepHours - idealSleepHours) +
          " hour(s) more sleep than you needed this week. You overslept."
      );
    } else {
      console.log(
        "You got " +
          (idealSleepHours - actualSleepHours) +
          " hour(s) less sleep than you needed this week. Get some more rest."
      );
    }
  }

calculateSleepDebt(); 