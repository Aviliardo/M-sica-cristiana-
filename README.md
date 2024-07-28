<!DOCTYPE html>
<html>
<head>
  <title>Aplicación de Música</title>
  <style>
    .album {
      margin: 20px;
      border: 1px solid #ccc;
      padding: 10px;
      cursor: pointer;
    }

    .album-title {
      font-weight: bold;
    }

    .songs {
      display: none;
      margin-left: 20px;
    }

    .song {
      margin-bottom: 5px;
    }

    .song-title {
      display: inline-block;
      width: 200px; /* Ajusta el ancho según sea necesario */
    }

    .song-image {
      width: 50px; /* Ajusta el ancho según sea necesario */
      height: 50px; /* Ajusta la altura según sea necesario */
      display: inline-block;
      margin-right: 10px;
    }
  </style>
</head>
<body>

  <h1>Mi Aplicación de Música</h1>

  <div class="album" onclick="showSongs('album1')">
    <div class="album-title">Álbum 1</div>
  </div>

  <div class="songs" id="album1">
    <div class="song">
      <img class="song-image" src="cancion1.jpg" alt="Canción 1">
      <div class="song-title">Canción 1</div>
      <audio controls>
        <source src="cancion1.mp3" type="audio/mpeg">
        Tu navegador no admite la reproducción de audio.
      </audio>
    </div>
    <div class="song">
      <img class="song-image" src="cancion2.jpg" alt="Canción 2">
      <div class="song-title">Canción 2</div>
      <audio controls>
        <source src="cancion2.mp3" type="audio/mpeg">
        Tu navegador no admite la reproducción de audio.
      </audio>
    </div>
  </div>

  <div class="album" onclick="showSongs('album2')">
    <div class="album-title">Álbum 2</div>
  </div>

  <div class="songs" id="album2">
    <div class="song">
      <img class="song-image" src="cancion3.jpg" alt="Canción 3">
      <div class="song-title">Canción 3</div>
      <audio controls>
        <source src="cancion3.mp3" type="audio/mpeg">
        Tu navegador no admite la reproducción de audio.
      </audio>
    </div>
    <div class="song">
      <img class="song-image" src="cancion4.jpg" alt="Canción 4">
      <div class="song-title">Canción 4</div>
      <audio controls>
        <source src="cancion4.mp3" type="audio/mpeg">
        Tu navegador no admite la reproducción de audio.
      </audio>
    </div>
  </div>

  <div class="album" onclick="showSongs('album3')">
    <div class="album-title">Álbum 3</div>
  </div>

  <div class="songs" id="album3">
    <div class="song">
      <img class="song-image" src="cancion5.jpg" alt="Canción 5">
      <div class="song-title">Canción 5</div>
      <audio controls>
        <source src="cancion5.mp3" type="audio/mpeg">
        Tu navegador no admite la reproducción de audio.
      </audio>
    </div>
    <div class="song">
      <img class="song-image" src="cancion6.jpg" alt="Canción 6">
      <div class="song-title">Canción 6</div>
      <audio controls>
        <source src="cancion6.mp3" type="audio/mpeg">
        Tu navegador no admite la reproducción de audio.
      </audio>
    </div>
  </div>

  <script>
    function showSongs(albumId) {
      var songs = document.getElementById(albumId);
      songs.style.display = songs.style.display === 'none' ? 'block' : 'none';
    }
  </script>

</body>
</html>
