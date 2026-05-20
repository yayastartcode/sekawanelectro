<svelte:head>
  <title>SekawanElectro | Jasa Service AC, Kulkas, Mesin Cuci & Elektronik</title>
  <meta name="description" content="SekawanElectro melayani cuci AC, service AC, bongkar pasang AC, service kulkas, mesin cuci, dan elektronik lain. Chat WhatsApp untuk panggil teknisi." />
</svelte:head>

<script>
  const phone = '6287814685027';
  const waText = encodeURIComponent('Halo SekawanElectro, saya mau konsultasi service AC/kulkas/mesin cuci.');
  const waLink = `https://wa.me/${phone}?text=${waText}`;

  const services = [
    { icon: '❄️', title: 'Cuci & Service AC', desc: 'Cuci AC, AC kurang dingin, bocor air, bau, berisik, isi freon, dan pengecekan unit.' },
    { icon: '🛠️', title: 'Bongkar Pasang AC', desc: 'Bongkar, pindah titik, pasang unit baru/lama, rapikan pipa dan jalur pembuangan.' },
    { icon: '🧊', title: 'Service Kulkas', desc: 'Kulkas tidak dingin, freezer bermasalah, bocor, bunyi tidak normal, dan pengecekan komponen.' },
    { icon: '🌀', title: 'Service Mesin Cuci', desc: 'Mesin cuci mati, tidak muter, error, bocor, pengering lemah, dan perawatan rutin.' },
    { icon: '⚡', title: 'Elektronik Lainnya', desc: 'Konsultasi perbaikan alat elektronik rumah tangga lain sesuai keluhan dan kondisi unit.' },
    { icon: '📍', title: 'Panggil Teknisi', desc: 'Chat lokasi, jenis unit, dan keluhan. Tim bantu arahkan estimasi dan jadwal kunjungan.' }
  ];

  const packages = [
    { name: 'Cek Keluhan', price: 'Chat dulu', detail: 'Kirim foto/video dan gejala kerusakan via WhatsApp.' },
    { name: 'Cuci AC', price: 'Estimasi cepat', detail: 'Untuk AC kotor, bau, netes, atau performa dingin menurun.' },
    { name: 'Service Unit', price: 'Sesuai kondisi', detail: 'Harga mengikuti jenis kerusakan, sparepart, dan lokasi pengerjaan.' }
  ];

  const process = [
    'Chat WhatsApp dan jelaskan keluhan unit',
    'Kirim foto/video, merek unit, dan lokasi',
    'Teknisi bantu estimasi dan atur jadwal',
    'Unit dicek, dikerjakan, lalu dites kembali'
  ];

  const faqs = [
    { q: 'Bisa panggil teknisi ke rumah?', a: 'Bisa. Kirim lokasi dan jenis perangkat dulu via WhatsApp untuk cek jadwal teknisi.' },
    { q: 'Bisa service AC yang tidak dingin?', a: 'Bisa. Penyebabnya bisa kotor, freon, kapasitor, kompresor, sensor, atau instalasi. Perlu dicek langsung.' },
    { q: 'Apakah bisa bongkar pasang AC?', a: 'Bisa. SekawanElectro melayani bongkar, pindah, dan pasang AC sesuai kondisi lokasi.' },
    { q: 'Harga pastinya berapa?', a: 'Harga tergantung jenis layanan, kerusakan, sparepart, dan lokasi. Chat dulu untuk estimasi awal.' }
  ];
</script>

<main class="min-h-screen bg-[#eef7f8] text-[#10212a]">
  <section class="relative overflow-hidden tech-grid">
    <div class="absolute inset-0 bg-gradient-to-br from-white/95 via-[#eef7f8]/92 to-[#d9f1f5]/86"></div>
    <div class="absolute -right-28 top-24 h-80 w-80 rounded-full bg-[#19a7ce]/25 blur-3xl"></div>
    <div class="absolute -left-24 bottom-16 h-72 w-72 rounded-full bg-[#ffb84d]/20 blur-3xl"></div>

    <nav class="relative z-10 mx-auto flex max-w-7xl items-center justify-between px-5 py-5 md:px-8">
      <a href="#top" class="flex items-center gap-3" aria-label="SekawanElectro home">
        <span class="grid h-12 w-12 place-items-center rounded-2xl bg-[#10212a] text-xl font-black text-[#7ee7ff] shadow-xl">SE</span>
        <span>
          <span class="block text-sm font-black uppercase tracking-[.2em] text-[#137c99]">SekawanElectro</span>
          <span class="block text-xs font-bold text-[#5b717a]">AC • Kulkas • Mesin Cuci</span>
        </span>
      </a>
      <div class="hidden items-center gap-7 text-sm font-black text-[#405962] md:flex">
        <a href="#layanan" class="hover:text-[#137c99]">Layanan</a>
        <a href="#paket" class="hover:text-[#137c99]">Estimasi</a>
        <a href="#proses" class="hover:text-[#137c99]">Proses</a>
        <a href="#faq" class="hover:text-[#137c99]">FAQ</a>
      </div>
      <a href={waLink} class="rounded-full bg-[#10212a] px-4 py-3 text-sm font-black text-white shadow-lg transition hover:-translate-y-0.5 hover:bg-[#193747]">Chat WA</a>
    </nav>

    <div id="top" class="relative z-10 mx-auto grid max-w-7xl gap-10 px-5 pb-20 pt-10 md:grid-cols-[1.05fr_.95fr] md:px-8 md:pb-28 md:pt-16">
      <div class="reveal-up max-w-3xl">
        <div class="mb-6 inline-flex items-center gap-2 rounded-full border border-[#b9e6ef] bg-white/70 px-4 py-2 text-sm font-black text-[#137c99] shadow-sm backdrop-blur">
          <span class="h-2 w-2 rounded-full bg-[#25D366]"></span>
          Teknisi elektronik rumah tangga - chat untuk jadwal
        </div>
        <h1 class="text-5xl font-black leading-[.96] tracking-[-.06em] text-[#10212a] md:text-7xl lg:text-8xl">
          AC dingin lagi, elektronik rumah beres lagi.
        </h1>
        <p class="mt-7 max-w-2xl text-lg leading-8 text-[#405962] md:text-xl">
          SekawanElectro melayani cuci AC, service AC, bongkar pasang AC, service kulkas, mesin cuci, dan elektronik lainnya. Jelaskan keluhan via WhatsApp, teknisi bantu cek estimasi dan jadwal.
        </p>
        <div class="mt-9 flex flex-col gap-3 sm:flex-row">
          <a href={waLink} class="rounded-full bg-[#25D366] px-7 py-4 text-center text-base font-black text-[#082414] shadow-xl shadow-[#25D366]/25 transition hover:-translate-y-1 hover:bg-[#1ebe5d]">Panggil Teknisi via WhatsApp</a>
          <a href="#layanan" class="rounded-full border border-[#10212a]/15 bg-white/70 px-7 py-4 text-center text-base font-black text-[#10212a] backdrop-blur transition hover:-translate-y-1 hover:bg-white">Lihat Layanan</a>
        </div>
        <div class="mt-10 grid max-w-2xl grid-cols-3 overflow-hidden rounded-[2rem] border border-[#10212a]/10 bg-white/70 shadow-sm backdrop-blur">
          <div class="p-4"><strong class="block text-2xl font-black text-[#137c99]">AC</strong><span class="text-xs font-bold text-[#5b717a]">Cuci & service</span></div>
          <div class="border-x border-[#10212a]/10 p-4"><strong class="block text-2xl font-black text-[#137c99]">24/7</strong><span class="text-xs font-bold text-[#5b717a]">Chat keluhan</span></div>
          <div class="p-4"><strong class="block text-2xl font-black text-[#137c99]">WA</strong><span class="text-xs font-bold text-[#5b717a]">Fast response</span></div>
        </div>
      </div>

      <div class="relative min-h-[520px] reveal-up" style="animation-delay: 140ms;">
        <div class="absolute right-0 top-6 h-[470px] w-[88%] rounded-[3rem] bg-[#10212a] shadow-2xl"></div>
        <div class="absolute left-0 top-0 w-[88%] overflow-hidden rounded-[3rem] border-[10px] border-white bg-[#d8f3f8] shadow-2xl">
          <div class="aspect-[4/5] bg-[radial-gradient(circle_at_24%_20%,#ffffff_0_10%,transparent_11%),linear-gradient(135deg,#dff8fc,#b7ebf5_45%,#fff0d3)]"></div>
          <div class="absolute inset-0 grid place-items-center p-8">
            <div class="w-full rounded-[2rem] bg-white/85 p-6 shadow-xl backdrop-blur">
              <div class="mb-5 flex items-center justify-between">
                <span class="rounded-full bg-[#e8f7fb] px-3 py-1 text-xs font-black uppercase tracking-[.16em] text-[#137c99]">Service Board</span>
                <span class="text-3xl">❄️</span>
              </div>
              <div class="space-y-3">
                {#each ['AC tidak dingin', 'Kulkas bermasalah', 'Mesin cuci error', 'Elektronik lain'] as item}
                  <div class="flex items-center justify-between rounded-2xl bg-[#f3fafb] px-4 py-3 font-black text-[#213943]"><span>{item}</span><span class="text-[#25D366]">✓</span></div>
                {/each}
              </div>
            </div>
          </div>
        </div>
        <div class="absolute bottom-10 right-2 max-w-[260px] rounded-[2rem] bg-[#ffb84d] p-5 text-[#10212a] shadow-2xl">
          <p class="text-sm font-black uppercase tracking-[.16em]">Tips cepat</p>
          <p class="mt-2 text-sm font-bold leading-6">Kirim foto unit + video keluhan agar estimasi lebih cepat.</p>
        </div>
      </div>
    </div>
  </section>

  <section id="layanan" class="px-5 py-20 md:px-8">
    <div class="mx-auto max-w-7xl">
      <div class="max-w-3xl">
        <p class="text-sm font-black uppercase tracking-[.24em] text-[#137c99]">Layanan utama</p>
        <h2 class="mt-3 text-4xl font-black tracking-[-.04em] md:text-6xl">Satu kontak untuk urusan elektronik rumah.</h2>
      </div>
      <div class="mt-10 grid gap-5 md:grid-cols-2 lg:grid-cols-3">
        {#each services as service}
          <article class="rounded-[2rem] border border-[#10212a]/10 bg-white p-6 shadow-sm transition hover:-translate-y-2 hover:shadow-2xl">
            <div class="mb-6 grid h-14 w-14 place-items-center rounded-2xl bg-[#e8f7fb] text-2xl">{service.icon}</div>
            <h3 class="text-2xl font-black tracking-[-.03em]">{service.title}</h3>
            <p class="mt-4 leading-7 text-[#516973]">{service.desc}</p>
          </article>
        {/each}
      </div>
    </div>
  </section>

  <section id="paket" class="bg-[#10212a] px-5 py-20 text-white md:px-8">
    <div class="mx-auto max-w-7xl">
      <div class="grid gap-10 md:grid-cols-[.9fr_1.1fr] md:items-start">
        <div>
          <p class="text-sm font-black uppercase tracking-[.24em] text-[#7ee7ff]">Estimasi awal</p>
          <h2 class="mt-3 text-4xl font-black tracking-[-.04em] md:text-6xl">Harga final setelah kondisi unit dicek.</h2>
          <p class="mt-5 text-lg leading-8 text-white/72">Untuk jasa service, biaya tergantung keluhan, lokasi, dan sparepart. Chat dulu agar teknisi bisa bantu estimasi awal.</p>
        </div>
        <div class="grid gap-4">
          {#each packages as item}
            <div class="rounded-[2rem] border border-white/10 bg-white/8 p-6 backdrop-blur">
              <div class="flex flex-col gap-3 sm:flex-row sm:items-center sm:justify-between">
                <h3 class="text-2xl font-black">{item.name}</h3>
                <span class="rounded-full bg-[#25D366] px-4 py-2 text-sm font-black text-[#082414]">{item.price}</span>
              </div>
              <p class="mt-3 leading-7 text-white/70">{item.detail}</p>
            </div>
          {/each}
        </div>
      </div>
    </div>
  </section>

  <section id="proses" class="px-5 py-20 md:px-8">
    <div class="mx-auto max-w-7xl">
      <div class="grid gap-10 md:grid-cols-[.85fr_1.15fr]">
        <div>
          <p class="text-sm font-black uppercase tracking-[.24em] text-[#137c99]">Cara order</p>
          <h2 class="mt-3 text-4xl font-black tracking-[-.04em] md:text-6xl">Mudah: chat, cek, jadwalkan.</h2>
          <a href={waLink} class="mt-8 inline-flex rounded-full bg-[#10212a] px-7 py-4 font-black text-white shadow-lg transition hover:-translate-y-1">Chat SekawanElectro</a>
        </div>
        <div class="space-y-4">
          {#each process as step, index}
            <div class="flex gap-5 rounded-[2rem] border border-[#10212a]/10 bg-white p-5 shadow-sm">
              <span class="grid h-12 w-12 shrink-0 place-items-center rounded-full bg-[#19a7ce] text-lg font-black text-white">{index + 1}</span>
              <p class="pt-2 text-lg font-bold leading-7 text-[#405962]">{step}</p>
            </div>
          {/each}
        </div>
      </div>
    </div>
  </section>

  <section class="px-5 pb-20 md:px-8">
    <div class="mx-auto max-w-7xl rounded-[3rem] bg-[#fff7e8] p-6 shadow-sm md:p-12">
      <div class="grid gap-8 md:grid-cols-[.82fr_1.18fr] md:items-center">
        <div>
          <p class="text-sm font-black uppercase tracking-[.24em] text-[#d58412]">Foto pengerjaan</p>
          <h2 class="mt-3 text-4xl font-black tracking-[-.04em] md:text-6xl">Dokumentasi kerja teknisi.</h2>
          <p class="mt-5 text-lg leading-8 text-[#6b5b45]">Lihat contoh pengerjaan cuci AC dan service kulkas. Kirim foto/video keluhan unit via WhatsApp supaya teknisi bisa bantu estimasi lebih cepat.</p>
          <a href={waLink} class="mt-8 inline-flex rounded-full bg-[#10212a] px-7 py-4 font-black text-white shadow-lg transition hover:-translate-y-1">Booking Teknisi</a>
        </div>
        <div class="grid gap-4 sm:grid-cols-2">
          <article class="group relative overflow-hidden rounded-[2.5rem] border-[10px] border-white bg-white shadow-2xl">
            <img
              src="/work/cuci-ac-pressure-wash.jpg"
              alt="Teknisi SekawanElectro membersihkan coil AC dengan spray air"
              class="aspect-[4/5] h-full w-full object-cover transition duration-500 group-hover:scale-105"
              loading="lazy"
            />
            <div class="absolute inset-x-4 bottom-4 rounded-[1.5rem] bg-[#10212a]/86 p-4 text-white shadow-xl backdrop-blur">
              <p class="text-xs font-black uppercase tracking-[.18em] text-[#7ee7ff]">Cuci AC</p>
              <p class="mt-1 text-base font-black">Pembersihan coil, filter, dan jalur buangan.</p>
            </div>
          </article>
          <article class="group relative overflow-hidden rounded-[2.5rem] border-[10px] border-white bg-white shadow-2xl sm:mt-10">
            <img
              src="/work/service-kulkas-repair.jpg"
              alt="Teknisi SekawanElectro memperbaiki bagian belakang kulkas"
              class="aspect-[4/5] h-full w-full object-cover transition duration-500 group-hover:scale-105"
              loading="lazy"
            />
            <div class="absolute inset-x-4 bottom-4 rounded-[1.5rem] bg-[#10212a]/86 p-4 text-white shadow-xl backdrop-blur">
              <p class="text-xs font-black uppercase tracking-[.18em] text-[#7ee7ff]">Service Kulkas</p>
              <p class="mt-1 text-base font-black">Pengecekan kompresor, kabel, dan komponen belakang unit.</p>
            </div>
          </article>
        </div>
      </div>
    </div>
  </section>

  <section id="faq" class="px-5 pb-20 md:px-8">
    <div class="mx-auto max-w-4xl">
      <p class="text-center text-sm font-black uppercase tracking-[.24em] text-[#137c99]">FAQ</p>
      <h2 class="mt-3 text-center text-4xl font-black tracking-[-.04em] md:text-6xl">Pertanyaan umum.</h2>
      <div class="mt-10 space-y-4">
        {#each faqs as faq}
          <details class="rounded-[1.5rem] border border-[#10212a]/10 bg-white p-5 shadow-sm">
            <summary class="cursor-pointer list-none text-lg font-black">{faq.q}</summary>
            <p class="mt-3 leading-7 text-[#516973]">{faq.a}</p>
          </details>
        {/each}
      </div>
    </div>
  </section>

  <section class="px-5 pb-8 md:px-8">
    <div class="mx-auto max-w-7xl rounded-[3rem] bg-[#19a7ce] p-8 text-white md:p-12">
      <div class="grid gap-8 md:grid-cols-[1fr_auto] md:items-center">
        <div>
          <h2 class="text-4xl font-black tracking-[-.04em] md:text-6xl">Butuh teknisi sekarang?</h2>
          <p class="mt-4 max-w-2xl text-lg font-bold leading-8 text-white/82">Chat WhatsApp, kirim keluhan unit, dan atur jadwal kunjungan teknisi SekawanElectro.</p>
        </div>
        <a href={waLink} class="rounded-full bg-[#10212a] px-8 py-5 text-center text-lg font-black text-white shadow-xl transition hover:-translate-y-1">WhatsApp 087814685027</a>
      </div>
    </div>
  </section>

  <footer class="px-5 pb-10 md:px-8">
    <div class="mx-auto flex max-w-7xl flex-col gap-4 border-t border-[#10212a]/10 pt-8 text-sm font-bold text-[#5b717a] md:flex-row md:items-center md:justify-between">
      <p>© 2026 SekawanElectro. Jasa service AC, kulkas, mesin cuci & elektronik.</p>
      <a class="hover:text-[#137c99]" href={waLink}>WhatsApp 087814685027</a>
    </div>
  </footer>

  <a href={waLink} class="pulse-ring fixed bottom-5 right-5 z-50 flex h-16 w-16 items-center justify-center rounded-full bg-[#25D366] text-white shadow-2xl shadow-[#25D366]/35 ring-4 ring-white/75 transition hover:-translate-y-1 hover:scale-105 focus:outline-none focus:ring-4 focus:ring-[#128C7E]/40 md:bottom-7 md:right-7 md:h-[72px] md:w-[72px]" aria-label="Chat SekawanElectro via WhatsApp">
    <svg viewBox="0 0 32 32" class="relative h-9 w-9" aria-hidden="true" fill="currentColor">
      <path d="M19.11 17.47c-.28-.14-1.66-.82-1.92-.91-.26-.1-.45-.14-.64.14-.19.28-.73.91-.9 1.1-.17.19-.33.21-.61.07-.28-.14-1.18-.43-2.24-1.38-.83-.74-1.39-1.65-1.55-1.93-.16-.28-.02-.43.12-.57.13-.13.28-.33.42-.49.14-.16.19-.28.28-.47.09-.19.05-.35-.02-.49-.07-.14-.64-1.55-.88-2.12-.23-.56-.47-.48-.64-.49h-.54c-.19 0-.49.07-.75.35-.26.28-.99.97-.99 2.36s1.01 2.74 1.15 2.93c.14.19 1.99 3.04 4.83 4.26.67.29 1.2.46 1.61.59.68.22 1.3.19 1.79.12.55-.08 1.66-.68 1.9-1.34.23-.66.23-1.22.16-1.34-.07-.12-.26-.19-.54-.33z" />
      <path d="M26.71 5.29A14.93 14.93 0 0 0 16.05.88C7.75.88 1 7.63 1 15.93c0 2.65.69 5.24 2 7.52L.88 31.12l7.86-2.06a15.02 15.02 0 0 0 7.31 1.86h.01c8.3 0 15.05-6.75 15.05-15.05 0-4.02-1.56-7.8-4.4-10.58zM16.06 28.38h-.01a12.5 12.5 0 0 1-6.36-1.74l-.46-.27-4.66 1.22 1.24-4.54-.3-.47a12.43 12.43 0 0 1-1.9-6.65c0-6.89 5.61-12.5 12.51-12.5 3.34 0 6.47 1.3 8.83 3.66a12.42 12.42 0 0 1 3.66 8.83c0 6.9-5.61 12.51-12.55 12.51z" />
    </svg>
  </a>
</main>
