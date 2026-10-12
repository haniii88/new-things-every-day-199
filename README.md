```javascript
function dailyLog199() {
  const habits = [
    { name: "Reading", completed: true },
    { name: "Exercise", completed: true },
    { name: "Coding", completed: false },
    { name: "Drinking Water", completed: true },
  ];

  const completed = habits.filter(habit => habit.completed);
  const rate = Math.round(
    (completed.length / habits.length) * 100
  );

  console.log("=== Daily Habit Report ===");
  console.log(`Completed: ${completed.length}/${habits.length}`);
  console.log(`Success Rate: ${rate}%`);

  habits.forEach(habit => {
    console.log(
      `${habit.completed ? "✅" : "❌"} ${habit.name}`
    );
  });
}

dailyLog199();
```
