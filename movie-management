const express = require("express");

const app = express();

app.use(express.json());

let movies = [
  {
    id: 1,
    title: "Pushpa",
    hero: "Allu Arjun"
  }
];

// Browser Test
app.get("/", (req, res) => {
  res.send("Movie API Running");
});

// Fetch Movies
app.get("/movies", (req, res) => {
  res.json(movies);
});

// Add Movie
app.post("/movies", (req, res) => {
  const movie = req.body;
  movies.push(movie);
  res.json({
    message: "Movie Added Successfully",
    data: movie
  });
});

app.listen(5000, () => {
  console.log("Server Running on Port 5000");
});
