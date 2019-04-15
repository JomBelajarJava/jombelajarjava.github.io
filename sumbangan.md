---
layout: page
title: Sumbangan
---

Website ini diusahakan sendiri oleh saya. Saya tidak ditaja oleh mana-mana
pihak. Sumbangan dan derma ikhlas dari anda sangat saya hargai sebagai tanda
sokongan anda terhadap usaha saya ini.

Anda boleh membuat sumbangan ke,

```
Bank: Maybank
Nombor akaun: 1580 5159 1340
Nama: Burhanuddin bin Baharuddin
```

Atau ke akaun paypal, [paypal.me/burhanloey][paypal].

Selepas membuat pembayaran, anda boleh menghantar email ke
[burhan@jombelajarjava.com][email] berserta bukti pembayaran supaya saya boleh
update jumlah derma yang terkumpul. Anda juga boleh sertakan sekali nama dan
pesanan untuk saya letakkan di website ini walaupun tidak wajib.

Jumlah derma setakat ini: RM 0.00

<p class="iframe-container has-text-centered">
  <a id="open-donation-form" class="button is-link">Buka borang untuk menghantar email</a>
</p>

<style>
  .loading {background:url(/assets/img/loading/loading.gif) center center no-repeat; background-size: 10% 10%;}
  iframe {height: 700px; border: none; overflow: hidden;}
</style>
<script>
  var iframeContainer = document.querySelector('.iframe-container');

  function openDonationForm(evt) {
    evt.preventDefault();
    var elem = evt.target;
    var iframe = document.createElement('iframe');
    iframe.setAttribute('class', 'block');
    iframe.setAttribute('src', 'https://app.jombelajarjava.com/donate');
    iframe.setAttribute('width', '800');
    iframe.setAttribute('scrolling', 'no');
    iframe.onload = function () {
        iframeContainer
            .setAttribute('class', 'iframe-container has-text-centered');
    };

    elem.parentNode.replaceChild(iframe, elem);

    iframeContainer
        .setAttribute('class', 'iframe-container has-text-centered loading');
  }

  document
      .querySelector('#open-donation-form')
      .addEventListener('click', openDonationForm);
</script>



[paypal]: https://paypal.me/burhanloey
[email]: mailto:burhan@jombelajarjava.com
