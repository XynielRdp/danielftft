<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FF CS TOURNAMENT - DANIEL NESIA</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&family=Inter:wght@400;600&display=swap');
        
        :root {
            --primary: #ef4444;
            --secondary: #f59e0b;
        }

        body { 
            font-family: 'Inter', sans-serif; 
            background-color: #0f172a; 
            color: white; 
            background-image: radial-gradient(circle at top right, rgba(239, 68, 68, 0.1), transparent),
                              radial-gradient(circle at bottom left, rgba(245, 158, 11, 0.05), transparent);
        }

        .font-esport { font-family: 'Orbitron', sans-serif; }
        
        .glass { 
            background: rgba(30, 41, 59, 0.7); 
            backdrop-filter: blur(12px); 
            border: 1px solid rgba(255, 255, 255, 0.08); 
        }

        .gradient-text { 
            background: linear-gradient(90deg, var(--secondary), var(--primary)); 
            -webkit-background-clip: text; 
            -webkit-text-fill-color: transparent; 
        }

        input:focus, textarea:focus {
            border-color: var(--primary) !important;
            box-shadow: 0 0 15px rgba(239, 68, 68, 0.3);
        }

        .btn-glow:hover {
            box-shadow: 0 0 20px rgba(239, 68, 68, 0.4);
            transform: translateY(-2px);
        }
    </style>
</head>
<body class="pb-10">

    <div class="relative h-72 flex items-center justify-center text-center px-4 overflow-hidden">
        <div class="absolute inset-0 bg-cover bg-center opacity-20 scale-110" style="background-image: url('https://files.catbox.moe/ihlasz.png');"></div>
        <div class="relative z-10">
            <div class="inline-block px-3 py-1 border border-red-500/50 rounded-full text-[10px] tracking-[4px] text-red-500 mb-4 bg-red-500/10 font-bold uppercase">
                Free Fire Clash Squad
            </div>
            <h1 class="text-4xl md:text-6xl font-black font-esport gradient-text tracking-tighter mb-2">TOURNAMENT</h1>
            <p class="text-gray-400 tracking-[0.3em] uppercase text-[10px]">Managed by Admin DANIEL NESIA</p>
        </div>
    </div>

    <div class="container max-w-2xl mx-auto px-4 -mt-12 relative z-20">
        
        <div class="grid grid-cols-2 gap-4 mb-6">
            <div class="glass p-5 rounded-2xl text-center border-t-2 border-yellow-500">
                <p class="text-[10px] text-gray-400 uppercase tracking-widest mb-1">Total Hadiah</p>
                <p class="text-3xl font-bold text-yellow-500 font-esport">40K</p>
                <p class="text-[9px] text-gray-500 mt-1 uppercase font-semibold">+ E-SERTIFIKAT</p>
            </div>
            <div class="glass p-5 rounded-2xl text-center border-t-2 border-red-500">
                <p class="text-[10px] text-gray-400 uppercase tracking-widest mb-1">Fee Register</p>
                <p class="text-3xl font-bold text-red-500 font-esport">5K</p>
                <p class="text-[9px] text-gray-500 mt-1 uppercase font-semibold">PER TEAM</p>
            </div>
        </div>

        <div class="glass p-8 rounded-[2.5rem] shadow-2xl border border-white/5">
            <div class="flex items-center justify-between mb-8">
                <h2 class="text-lg font-bold font-esport flex items-center">
                    <span class="w-2 h-8 bg-red-600 mr-3 rounded-full"></span>
                    REGISTRASI TIM
                </h2>
                <i class="fas fa-trophy text-yellow-600 text-xl opacity-50"></i>
            </div>
            
            <form id="tourneyForm" class="space-y-5">
                <div class="group">
                    <label class="block text-[10px] font-bold text-gray-500 mb-2 tracking-widest ml-1 uppercase">Nama Team</label>
                    <input type="text" id="teamName" required placeholder="Masukkan Nama Tim..." 
                        class="w-full bg-slate-900/50 border border-slate-800 rounded-2xl px-5 py-4 outline-none transition-all placeholder:text-gray-700">
                </div>

                <div class="group">
                    <label class="block text-[10px] font-bold text-gray-500 mb-2 tracking-widest ml-1 uppercase">Nama Kapten (In-Game)</label>
                    <input type="text" id="captainName" required placeholder="Nickname Kapten..." 
                        class="w-full bg-slate-900/50 border border-slate-800 rounded-2xl px-5 py-4 outline-none transition-all placeholder:text-gray-700">
                </div>

                <div class="group">
                    <label class="block text-[10px] font-bold text-gray-500 mb-2 tracking-widest ml-1 uppercase">WhatsApp Aktif</label>
                    <input type="number" id="waNumber" required placeholder="08xxxxxxxxxx" 
                        class="w-full bg-slate-900/50 border border-slate-800 rounded-2xl px-5 py-4 outline-none transition-all placeholder:text-gray-700">
                </div>

                <div class="group">
                    <label class="block text-[10px] font-bold text-gray-500 mb-2 tracking-widest ml-1 uppercase">List Anggota (Nama / ID)</label>
                    <textarea id="members" rows="4" required placeholder="1. Nick / ID&#10;2. Nick / ID&#10;3. Nick / ID&#10;4. Nick / ID" 
                        class="w-full bg-slate-900/50 border border-slate-800 rounded-2xl px-5 py-4 outline-none transition-all placeholder:text-gray-700 resize-none"></textarea>
                </div>

                <div class="pt-4">
                    <button type="submit" 
                        class="btn-glow w-full bg-gradient-to-r from-red-600 to-orange-600 text-white font-bold py-5 rounded-2xl shadow-[0_10px_20px_rgba(220,38,38,0.2)] flex items-center justify-center gap-3 transition-all duration-300">
                        <span class="uppercase tracking-widest text-sm">Daftar Sekarang</span>
                        <i class="fab fa-whatsapp text-xl"></i>
                    </button>
                </div>
            </form>
        </div>

        <div class="mt-8 glass p-6 rounded-3xl border border-white/5">
            <h3 class="font-bold text-sm mb-4 text-orange-500 flex items-center uppercase tracking-widest font-esport">
                <i class="fas fa-scroll mr-2"></i> Aturan Main
            </h3>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-3">
                <div class="flex items-center text-[11px] text-gray-400 bg-white/5 p-3 rounded-xl">
                    <i class="fas fa-mobile-alt text-red-500 mr-3"></i> MOBILE ONLY
                </div>
                <div class="flex items-center text-[11px] text-gray-400 bg-white/5 p-3 rounded-xl">
                    <i class="fas fa-ban text-red-500 mr-3"></i> NO EMULATOR
                </div>
                <div class="flex items-center text-[11px] text-gray-400 bg-white/5 p-3 rounded-xl">
                    <i class="fas fa-shield-alt text-red-500 mr-3"></i> SKIN ON / GUN OFF
                </div>
                <div class="flex items-center text-[11px] text-gray-400 bg-white/5 p-3 rounded-xl">
                    <i class="fas fa-clock text-red-500 mr-3"></i> ON TIME
                </div>
            </div>
        </div>

        <div class="text-center mt-12">
            <p class="text-[10px] text-gray-600 uppercase tracking-[4px]">Powered by Daniel Nesia & Han</p>
        </div>
    </div>

    <script>
        document.getElementById('tourneyForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // KONFIGURASI ADMIN
            const adminWA = "6285814412482"; 
            
            // AMBIL DATA INPUT
            const team = document.getElementById('teamName').value.toUpperCase();
            const captain = document.getElementById('captainName').value;
            const wa = document.getElementById('waNumber').value;
            const listMember = document.getElementById('members').value;

            // FORMAT PESAN WHATSAPP
            const message = `*PENDAFTARAN TOURNAMENT FF CS*%0A` +
                            `------------------------------------------%0A` +
                            `*🔥 Nama Team:* ${team}%0A` +
                            `*👑 Kapten:* ${captain}%0A` +
                            `*📱 WhatsApp:* ${wa}%0A%0A` +
                            `*🎮 List Anggota:*%0A${encodeURIComponent(listMember)}%0A` +
                            `------------------------------------------%0A` +
                            `*💰 TOTAL BAYAR: Rp 5.000*%0A%0A` +
                            `_Saya setuju dengan aturan yang berlaku. Mohon kirimkan nomor tujuan pembayaran._`;

            // EKSEKUSI KIRIM KE WA
            window.open(`https://wa.me/${adminWA}?text=${message}`, '_blank');
        });
    </script>
</body>
</html>
