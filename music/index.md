# Музыка

Здесь представлены фрагменты моих работ.

### Xen

<audio src="assets/xen.wav" controls loop></audio>

### Солнечный ветер

<audio src="/projects/solar-wind/assets/solar-wind.wav" controls loop></audio>

### Aqua

<audio src="assets/aqua.wav" controls loop></audio>

<script>
  const audios = document.querySelectorAll('audio');

  audios.forEach(audio => {
    audio.addEventListener('play', () => {
      audios.forEach(otherAudio => {
        if (otherAudio !== audio) {
          otherAudio.pause();
        }
      });
    });
  });
</script>
