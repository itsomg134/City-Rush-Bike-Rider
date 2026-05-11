#  City Rush: Bike Rider

**Dodge traffic, set high scores, and survive the urban jungle!**  
City Rush is an fast-paced, lane-based bike dodging game built with pure HTML, CSS, and JavaScript. Avoid incoming red cars, survive as long as possible, and beat your personal best.

![Game Screenshot](https://via.placeholder.com/800x400?text=City+Rush+Gameplay+Preview)  
*(Add a real screenshot of your game here for the best effect)*

##  Play Now

You can play the game directly in your browser:  
 **[Click here to play City Rush: Bike Rider](https://your-username.github.io/bike-game)**  
*(Replace the link with your actual GitHub Pages URL after deploying)*

##  Features

-  **Smooth Lane-based Movement** – 5 lanes of action, easy to control.
-  **Dynamic Difficulty** – Cars move faster and spawn more frequently as your score increases.
-  **Persistent High Score** – Your best score is saved locally in your browser.
-  **Stylish Pixel Art** – Detailed bike sprite, animated cars, and a gritty road aesthetic.
-  **Mobile & Touch Friendly** – On-screen buttons for left/right movement, plus full keyboard support (A/D or Arrow Keys).
-  **Real-time Scoring** – Earn points for survival and bonus points for every car you safely pass.

##  How to Play

- **Goal:** Avoid the red cars for as long as possible.
- **Controls:**
    - **Keyboard:** Press `A` / `←` (Left Arrow) to move left, `D` / `→` (Right Arrow) to move right.
    - **Mouse/Touch:** Click the `◀ LEFT` and `RIGHT ` buttons on the screen.
    - **Restart:** Press `R` on your keyboard or click the ` RESTART` button.

- **Scoring:**
    - You gain `0.25` points every frame just for surviving.
    - You get a `+8` point bonus every time a car safely passes below you.
    - The game ends instantly upon collision with any car.

##  Technologies Used

- **HTML5 Canvas** – For rendering the game graphics.
- **CSS3** – For styling the UI, buttons, and responsive layout.
- **Vanilla JavaScript (ES6)** – For all game logic, collision detection, movement, and dynamic difficulty.
- **LocalStorage API** – To save and load the player's best score.

##  Installation & Running Locally

You can run this game on any modern web server or even directly from your local file system.

### Option 1: Simple Local Run

1.  **Download the code:** Save the provided `index.html` file to your computer.
2.  **Double-click:** Open the file with your web browser (Chrome, Firefox, Edge, etc.).
3.  **Play!** No additional setup required.

### Option 2: Run with a Local Server (Recommended for developers)

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/bike-game.git
    cd bike-game
    ```
2.  **Start a simple server:** (using Python)
    ```bash
    # Python 3
    python -m http.server 8000
    ```
3.  **Open your browser** and go to `http://localhost:8000`.

## 📁 Project Structure

Since the game is contained in a single HTML file, the project is extremely lightweight:

```
bike-game/
│
└── index.html      # Contains all HTML, CSS, and JavaScript
```

##  Game Logic Overview

- **Canvas Rendering:** The game runs at ~60 FPS using `requestAnimationFrame`.
- **Collision Detection:** Axis-Aligned Bounding Box (AABB) collision between the player's bike and enemy cars.
- **Traffic System:** Cars are spawned at random intervals and lanes. Their downward speed increases with the player's score.
- **Difficulty Scaling:**
    - `currentCarSpeed` increases based on `score`.
    - `spawnDelay` decreases based on `score`, making cars appear more frequently.
- **Persistent Storage:** The best score is saved after each game over and loaded when the page loads.

##  Customization

Want to tweak the game? Open `index.html` in a code editor and modify these variables:

- **`LANE_COUNT`** – Change the number of lanes (default is 5).
- **`baseCarSpeed`** – The starting speed of enemy cars (default 2.6).
- **`baseSpawnDelay`** – How often cars spawn in frames (default 45).
- **Colors & Sizes:** Adjust `PLAYER_WIDTH`, `CAR_WIDTH`, or the color codes inside `drawCar()` and `drawBike()`.

## 🐛 Known Issues & Limitations

- Very high scores may cause extreme difficulty (cars become very fast). This is intentional as an "endless challenge".
- On very small mobile screens (< 320px width), the control buttons might overlap slightly. Use landscape mode for the best experience.

## 🔮 Future Ideas

- Add sound effects for passing cars and collisions.
- Introduce different enemy types (trucks, motorcycles) with varying sizes/speeds.
- Add power-ups (slow motion, invincibility, score multiplier).
- Implement a "night mode" with dynamic lighting.

## 🤝 Contributing

Contributions are welcome! If you have ideas for improvements or find a bug, feel free to:

1.  Fork the repository.
2.  Create your feature branch (`git checkout -b feature/amazing-idea`).
3.  Commit your changes (`git commit -m 'Add some amazing feature'`).
4.  Push to the branch (`git push origin feature/amazing-idea`).
5.  Open a Pull Request.

##  License

This project is open-source and available under the **MIT License**. You are free to use, modify, and distribute it as you like.

---

##  Contact

Created by **Your Name** – feel free to reach out!

- GitHub: [@your-username](https://github.com/your-username)
- Project Link: [https://github.com/your-username/bike-game](https://github.com/your-username/bike-game
