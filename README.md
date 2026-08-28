<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Your Perfect Day Routine</title>
  <style>
    /* Global Styles */
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    body {
      background-color: #f7fafc;
      color: #2d3748;
      line-height: 1.6;
    }

    /* Centered Hero Section */
    .hero {
      background: linear-gradient(135deg, #4f46e5, #7c3aed);
      color: #ffffff;
      padding: 5rem 2rem;
      text-align: center;
    }

    .hero h1 {
      font-size: 3rem;
      margin-bottom: 1rem;
      letter-spacing: -0.5px;
    }

    .hero p {
      font-size: 1.2rem;
      max-width: 650px;
      margin: 0.5rem auto;
      opacity: 0.95;
    }

    /* Layout Containers */
    .container {
      max-width: 900px;
      margin: 0 auto;
      padding: 3rem 1.5rem;
    }

    .card {
      background: #ffffff;
      border-radius: 12px;
      padding: 2.5rem;
      margin-bottom: 2.5rem;
      box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
    }

    h2 {
      font-size: 1.75rem;
      color: #1a202c;
      margin-bottom: 1.5rem;
      border-left: 4px solid #4f46e5;
      padding-left: 0.75rem;
    }

    /* Section 1: Morning Mindset Cards */
    .mindset-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
      gap: 1.25rem;
      margin-top: 1rem;
    }

    .mindset-item {
      background: #f8fafc;
      border: 1px solid #e2e8f0;
      border-radius: 8px;
      padding: 1.25rem;
    }

    .mindset-item h4 {
      color: #4f46e5;
      margin-bottom: 0.5rem;
      font-size: 1.1rem;
    }

    /* Section 2: Full-Day Detailed Timeline */
    .timeline {
      display: flex;
      flex-direction: column;
      gap: 1.5rem;
    }

    .time-block {
      display: flex;
      gap: 1.5rem;
      align-items: flex-start;
      border-bottom: 1px solid #edf2f7;
      padding-bottom: 1.25rem;
    }

    .time-block:last-child {
      border-bottom: none;
      padding-bottom: 0;
    }

    .badge {
      background: #e0e7ff;
      color: #4338ca;
      font-weight: 700;
      font-size: 0.85rem;
      padding: 0.4rem 0.8rem;
      border-radius: 20px;
      white-space: nowrap;
    }

    .time-details h3 {
      font-size: 1.15rem;
      margin-bottom: 0.25rem;
    }

    .time-details p {
      color: #718096;
      font-size: 0.95rem;
    }

    /* Section 3: Interactive To-Do List */
    .todo-list {
      list-style: none;
    }

    .todo-item {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 1rem 0.75rem;
      border-bottom: 1px solid #edf2f7;
      transition: background-color 0.2s;
    }

    .todo-item:hover {
      background-color: #f8fafc;
    }

    .todo-item:last-child {
      border-bottom: none;
    }

    .todo-left {
      display: flex;
      align-items: center;
      gap: 1rem;
    }

    /* Checkbox & Strikethrough Logic */
    .todo-item input[type="checkbox"] {
      width: 22px;
      height: 22px;
      accent-color: #4f46e5;
      cursor: pointer;
    }

    .todo-item input[type="checkbox"]:checked + label {
      text-decoration: line-through;
      color: #a0aec0;
    }

    .todo-item label {
      font-size: 1.05rem;
      cursor: pointer;
      font-weight: 500;
    }

    .category-tag {
      font-size: 0.75rem;
      text-transform: uppercase;
      letter-spacing: 0.5px;
      padding: 0.2rem 0.6rem;
      border-radius: 4px;
      background: #edf2f7;
      color: #4a5568;
    }

    /* Section 4: Final Motivation Banner */
    .motivation-banner {
      background: linear-gradient(135deg, #1e293b, #0f172a);
      color: #ffffff;
      border-radius: 12px;
      padding: 3rem 2rem;
      text-align: center;
      margin-bottom: 2.5rem;
      box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
    }

    .motivation-banner h2 {
      border: none;
      color: #38bdf8;
      font-size: 2rem;
      margin-bottom: 1rem;
      padding: 0;
    }

    .motivation-banner p {
      font-size: 1.15rem;
      max-width: 700px;
      margin: 0.8rem auto;
      color: #e2e8f0;
      line-height: 1.7;
    }

    .motivation-highlight {
      color: #facc15;
      font-weight: 600;
    }

    /* Footer */
    footer {
      text-align: center;
      padding: 2.5rem 1.5rem;
      background-color: #0f172a;
      color: #94a3b8;
      font-size: 1rem;
      border-top: 1px solid #1e293b;
    }

    footer .author {
      color: #38bdf8;
      font-weight: bold;
      font-size: 1.2rem;
      letter-spacing: 1px;
      margin-top: 0.5rem;
      display: block;
    }
  </style>
</head>
<body>

  <header class="hero">
    <h1>Your Perfect Day</h1>
    <p>Win the morning, own the afternoon, and restore in the evening.</p>
    <p>A structured blueprint to turn daily effort into momentum.</p>
  </header>

  <main class="container">

    <section class="card">
      <h2>First Steps Upon Waking</h2>
      <p style="color: #4a5568; margin-bottom: 1rem;">Do these three things before touching your phone or checking notifications:</p>
      
      <div class="mindset-grid">
        <div class="mindset-item">
          <h4>1. Hydrate & Breathe</h4>
          <p>Drink a full glass of water immediately to wake up your body. Take 5 deep breaths.</p>
        </div>
        <div class="mindset-item">
          <h4>2. Morning Intent</h4>
          <p>Remind yourself: "Today is a clear slate. I focus only on what I can control."</p>
        </div>
        <div class="mindset-item">
          <h4>3. Daylight Exposure</h4>
          <p>Step outside or open a window for natural light to set your circadian rhythm.</p>
        </div>
      </div>
    </section>

    <section class="card">
      <h2>Full Day Master Routine</h2>
      <div class="timeline">
        
        <div class="time-block">
          <span class="badge">06:30 AM - 08:00 AM</span>
          <div class="time-details">
            <h3>Morning Prime</h3>
            <p>Hydrate, light physical movement, outdoor sun exposure, and a nutritious breakfast.</p>
          </div>
        </div>

        <div class="time-block">
          <span class="badge">08:00 AM - 12:00 PM</span>
          <div class="time-details">
            <h3>Deep Focus Window</h3>
            <p>Tackle your single hardest priority task while your energy and willpower are highest.</p>
          </div>
        </div>

        <div class="time-block">
          <span class="badge">12:00 PM - 01:30 PM</span>
          <div class="time-details">
            <h3>Midday Reset</h3>
            <p>Eat a balanced lunch, take a step away from screens, and get a short walk outside.</p>
          </div>
        </div>

        <div class="time-block">
          <span class="badge">01:30 PM - 05:00 PM</span>
          <div class="time-details">
            <h3>Execution & Admin</h3>
            <p>Handle meetings, emails, collaborative work, and secondary routine tasks.</p>
          </div>
        </div>

        <div class="time-block">
          <span class="badge">05:00 PM - 08:00 PM</span>
          <div class="time-details">
            <h3>Personal Time & Exercise</h3>
            <p>Work out, engage with hobbies, cook dinner, and spend time with family or friends.</p>
          </div>
        </div>

        <div class="time-block">
          <span class="badge">08:00 PM - 10:30 PM</span>
          <div class="time-details">
            <h3>Night Wind-Down</h3>
            <p>Dim the lights, turn off screens, review tomorrow's goals, and prepare for rest.</p>
          </div>
        </div>

      </div>
    </section>

    <section class="card">
      <h2>Daily Action Checklist</h2>
      <p style="color: #4a5568; margin-bottom: 1.5rem;">Tick each task off as you complete it throughout the day:</p>

      <ul class="todo-list">
        <li class="todo-item">
          <div class="todo-left">
            <input type="checkbox" id="task1">
            <label for="task1">Drink 500ml of water upon waking</label>
          </div>
          <span class="category-tag">Morning</span>
        </li>

        <li class="todo-item">
          <div class="todo-left">
            <input type="checkbox" id="task2">
            <label for="task2">Complete 20 minutes of physical exercise</label>
          </div>
          <span class="category-tag">Morning</span>
        </li>

        <li class="todo-item">
          <div class="todo-left">
            <input type="checkbox" id="task3">
            <label for="task3">Finish #1 primary goal for the day</label>
          </div>
          <span class="category-tag">Focus</span>
        </li>

        <li class="todo-item">
          <div class="todo-left">
            <input type="checkbox" id="task4">
            <label for="task4">Take a 15-minute afternoon walking break</label>
          </div>
          <span class="category-tag">Reset</span>
        </li>

        <li class="todo-item">
          <div class="todo-left">
            <input type="checkbox" id="task5">
            <label for="task5">Read 10 pages of a book</label>
          </div>
          <span class="category-tag">Evening</span>
        </li>

        <li class="todo-item">
          <div class="todo-left">
            <input type="checkbox" id="task6">
            <label for="task6">Turn off screens 1 hour before sleep</label>
          </div>
          <span class="category-tag">Evening</span>
        </li>
      </ul>
    </section>

    <section class="motivation-banner">
      <h2>Keep Going & Stay Refreshed</h2>
      <p>Keep your day good, positive, and focused. Incorporate <span class="motivation-highlight">more exercise</span> into your daily routine to boost your energy, clear your mind, and build lasting strength.</p>
      <p>Make your routine better every single day. Stay refreshed, stay hydrated, and continuous progress will follow!</p>
      <p style="font-style: italic; margin-top: 1.2rem; color: #94a3b8;">"Small discipline repeated daily leads to great achievements over time."</p>
    </section>

  </main>

  <footer>
    <p>Designed & Created by</p>
    <span class="author">MUZAINA MUSTAAN</span>
    <p style="margin-top: 0.5rem; font-size: 0.85rem;">&copy; 2026 Your Perfect Day Project</p>
  </footer>

</body>
</html>
