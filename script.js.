document.addEventListener('DOMContentLoaded', function() {
    // Swiper Slider
    var swiper = new Swiper('.swiper-container', {
        slidesPerView: 1,
        spaceBetween: 20,
        loop: true,
        pagination: { el: '.swiper-pagination', clickable: true },
        navigation: { nextEl: '.swiper-button-next', prevEl: '.swiper-button-prev' },
        autoplay: { delay: 4000, disableOnInteraction: false }
    });

    // Müzik Çalar Aç/Kapa
    document.querySelector('.music-player').addEventListener('click', function() {
        this.classList.toggle('active');
    });

    // Blog İçeriği Genişletme/Küçültme
    window.toggleContent = function(id) {
        var content = document.getElementById(id);
        content.classList.toggle('active');
        var btn = document.querySelector(`button[onclick="toggleContent('${id}')"]`);
        btn.textContent = content.classList.contains('active') ? 'Küçült' : 'Devamını Oku';
    };

    // Yükleme Animasyonu
    window.addEventListener('load', function() {
        document.querySelector('.loader').classList.remove('active');
    });
    document.querySelector('.loader').classList.add('active');
});
