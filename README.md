const express = require("express");
const app = express();

app.get("/", (req, res) => {
  res.send("🎰 ¡Servidor de tragamonedas con fichas funcionando!");
});

const PORT = process.env.PORT || 3000;
app.listen(PORT, () => {
  console.log(`Servidor corriendo en puerto ${PORT}`);
});
