<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Alasonatti Scavi | Movimento Terra e Lavori Forestali a Pessinetto</title>
    <meta name="description" content="Alasonatti Scavi: impresa a gestione familiare da 4 generazioni specializzata in scavi, lavori forestali, sgombero neve e fognature a Pessinetto (TO).">
    
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;800&family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        brand: {
                            orange: '#FF6600', // Arancione stile Hitachi
                            blue: '#002D62',   // Blu aziendale
                            black: '#0a0a0a',  // Nero per fondi logo
                            gray: '#374151',
                            light: '#F3F4F6'
                        }
                    },
                    fontFamily: {
                        heading: ['Montserrat', 'sans-serif'],
                        body: ['Open Sans', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>

    <style>
        /* Smooth scrolling */
        html { scroll-behavior: smooth; }
        
        /* Custom image overlay */
        .hero-overlay {
            background: linear-gradient(to right, rgba(0, 45, 98, 0.8) 0%, rgba(10, 10, 10, 0.6) 100%);
        }
    </style>
</head>
<body class="font-body text-gray-800 bg-brand-light">

    <!-- Navigation -->
    <nav class="fixed w-full z-50 bg-brand-black/95 backdrop-blur-sm text-white shadow-lg transition-all duration-300">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-24">
                <!-- Logo -->
                <div class="flex-shrink-0 flex items-center cursor-pointer py-2" onclick="window.scrollTo(0,0)">
                    <img src="alasonatti logo compl copia 2.jpg" alt="Alasonatti Scavi Logo" class="h-20 w-auto object-contain">
                </div>
                
                <!-- Desktop Menu -->
                <div class="hidden md:flex space-x-8 items-center">
                    <a href="#chi-siamo" class="hover:text-brand-orange transition font-semibold">Chi Siamo</a>
                    <a href="#servizi" class="hover:text-brand-orange transition font-semibold">Servizi</a>
                    <a href="#instagram" class="hover:text-brand-orange transition font-semibold">Gallery</a>
                    <a href="#contatti" class="bg-brand-orange text-white px-6 py-2 rounded-md font-bold hover:bg-orange-500 transition shadow-md">Richiedi Preventivo</a>
                </div>

                <!-- Mobile menu button -->
                <div class="md:hidden flex items-center">
                    <button id="mobile-menu-btn" class="text-white hover:text-brand-orange focus:outline-none">
                        <i data-lucide="menu" class="w-8 h-8"></i>
                    </button>
                </div>
            </div>
        </div>

        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-brand-black border-t border-gray-800">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3 text-center">
                <a href="#chi-siamo" class="block px-3 py-2 text-base font-medium hover:text-brand-orange mobile-link">Chi Siamo</a>
                <a href="#servizi" class="block px-3 py-2 text-base font-medium hover:text-brand-orange mobile-link">Servizi</a>
                <a href="#instagram" class="block px-3 py-2 text-base font-medium hover:text-brand-orange mobile-link">Gallery</a>
                <a href="#contatti" class="block px-3 py-2 text-base font-medium text-brand-orange mobile-link">Contatti</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="relative h-screen flex items-center justify-center pt-24">
        <!-- Background Image (Escavatore in natura) -->
        <div class="absolute inset-0 z-0">
            <img src="https://images.unsplash.com/photo-1621251919864-16a3e7db0160?q=80&w=2070&auto=format&fit=crop" 
                 alt="[Immagine di un escavatore immerso nella natura]" 
                 class="w-full h-full object-cover">
            <div class="absolute inset-0 hero-overlay"></div>
        </div>

        <div class="relative z-10 text-center px-4 max-w-5xl mx-auto">
            <h1 class="font-heading font-800 text-4xl sm:text-5xl md:text-6xl text-white mb-6 uppercase tracking-tight leading-tight">
                L'esperienza di 4 generazioni,<br>
                <span class="text-brand-orange">al servizio del territorio.</span>
            </h1>
            <p class="text-lg sm:text-xl text-gray-200 mb-10 max-w-3xl mx-auto font-light leading-relaxed">
                Dal movimento terra alle opere forestali, dagli acquedotti allo sgombero neve. Lavoriamo ogni giorno con passione e competenza per consegnare lavori fatti a regola d'arte.
            </p>
            <div class="flex flex-col sm:flex-row gap-4 justify-center">
                <a href="#contatti" class="bg-brand-orange text-white font-bold text-lg px-8 py-4 rounded hover:bg-orange-500 transition transform hover:-translate-y-1 shadow-lg flex items-center justify-center gap-2">
                    <i data-lucide="phone-call" class="w-5 h-5"></i> 0123504231
                </a>
                <a href="#servizi" class="bg-brand-blue border border-brand-blue text-white font-bold text-lg px-8 py-4 rounded hover:bg-blue-800 transition transform hover:-translate-y-1 flex items-center justify-center gap-2 shadow-lg">
                    Scopri i Servizi
                </a>
            </div>
        </div>
    </section>

    <!-- Chi Siamo Section -->
    <section id="chi-siamo" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
                <div>
                    <h2 class="font-heading font-800 text-3xl md:text-4xl text-brand-blue mb-6">La nostra Storia, il nostro Lavoro</h2>
                    <div class="w-20 h-2 bg-brand-orange mb-6"></div>
                    <p class="text-gray-600 mb-4 text-lg leading-relaxed">
                        Situata a Pessinetto (Fraz. Losa), <strong>Alasonatti Scavi</strong> è un'azienda a <strong>gestione familiare giunta alla sua quarta generazione</strong>. Una tradizione tramandata di padre in figlio che unisce l'antica passione per il territorio alle competenze tecniche necessarie per affrontare ogni tipo di cantiere.
                    </p>
                    <p class="text-gray-600 mb-6 text-lg leading-relaxed">
                        Il nostro obiettivo principale è <strong>lavorare bene</strong>. Eseguiamo ogni intervento con la massima cura e precisione, dall'opera pubblica al lavoro per il privato. Conosciamo profondamente il nostro territorio montano e operiamo con serietà per garantire risultati duraturi e sicuri, mantenendo sempre un occhio di riguardo al rispetto dell'ambiente.
                    </p>
                    <ul class="space-y-3">
                        <li class="flex items-center gap-3 text-brand-blue font-semibold">
                            <i data-lucide="history" class="text-brand-orange w-6 h-6"></i> Gestione familiare e affidabilità da 4 generazioni
                        </li>
                        <li class="flex items-center gap-3 text-brand-blue font-semibold">
                            <i data-lucide="check-circle-2" class="text-brand-orange w-6 h-6"></i> Massima cura, precisione e lavori a regola d'arte
                        </li>
                        <li class="flex items-center gap-3 text-brand-blue font-semibold">
                            <i data-lucide="leaf" class="text-brand-orange w-6 h-6"></i> Rispetto per il territorio e l'ambiente circostante
                        </li>
                    </ul>
                </div>
                <div class="relative">
                    <div class="absolute inset-0 bg-brand-orange transform translate-x-4 translate-y-4 rounded-lg"></div>
                    <img src="https://images.unsplash.com/photo-1542601906990-b4d3fb778b09?q=80&w=2026&auto=format&fit=crop" 
                         alt="[Natura e macchinari al lavoro]" 
                         class="relative z-10 rounded-lg shadow-xl w-full h-auto object-cover"
                         style="max-height: 500px;">
                </div>
            </div>
        </div>
    </section>

    <!-- Servizi Section -->
    <section id="servizi" class="py-20 bg-brand-light">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="font-heading font-800 text-3xl md:text-4xl text-brand-blue mb-4">Aree di Intervento</h2>
                <div class="w-20 h-2 bg-brand-orange mx-auto mb-4"></div>
                <p class="text-gray-600 max-w-2xl mx-auto">Interventi specializzati per l'ambiente, l'urbanistica e le opere civili, eseguiti con la massima competenza.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Servizio 1 -->
                <div class="bg-white p-8 rounded-xl shadow-md hover:shadow-xl transition duration-300 border-b-4 border-transparent hover:border-brand-orange group">
                    <div class="bg-brand-light w-16 h-16 rounded-full flex items-center justify-center mb-6 group-hover:bg-brand-orange group-hover:text-white transition text-brand-blue">
                        <i data-lucide="snowflake" class="w-8 h-8"></i>
                    </div>
                    <h3 class="font-heading font-bold text-xl mb-3 text-brand-blue">Sgombero Neve</h3>
                    <p class="text-gray-600">Servizio tempestivo e professionale di pulizia strade, piazzali e viabilità locale dalla neve, fondamentale durante l'inverno nelle nostre valli.</p>
                </div>

                <!-- Servizio 2 -->
                <div class="bg-white p-8 rounded-xl shadow-md hover:shadow-xl transition duration-300 border-b-4 border-transparent hover:border-brand-orange group">
                    <div class="bg-brand-light w-16 h-16 rounded-full flex items-center justify-center mb-6 group-hover:bg-brand-orange group-hover:text-white transition text-brand-blue">
                        <i data-lucide="droplets" class="w-8 h-8"></i>
                    </div>
                    <h3 class="font-heading font-bold text-xl mb-3 text-brand-blue">Costruzione Acquedotti e Fognature</h3>
                    <p class="text-gray-600">Realizzazione completa, posa e manutenzione di reti idriche e fognarie. Interventi precisi per garantire reti sicure, efficienti e durature nel tempo.</p>
                </div>

                <!-- Servizio 3 -->
                <div class="bg-white p-8 rounded-xl shadow-md hover:shadow-xl transition duration-300 border-b-4 border-transparent hover:border-brand-orange group">
                    <div class="bg-brand-light w-16 h-16 rounded-full flex items-center justify-center mb-6 group-hover:bg-brand-orange group-hover:text-white transition text-brand-blue">
                        <i data-lucide="waves" class="w-8 h-8"></i>
                    </div>
                    <h3 class="font-heading font-bold text-xl mb-3 text-brand-blue">Realizzazione Disalvei</h3>
                    <p class="text-gray-600">Opere di sistemazione idrogeologica, pulizia dei letti fluviali, costruzione di scogliere e argini per la prevenzione dei rischi idrogeologici.</p>
                </div>

                <!-- Servizio 4 -->
                <div class="bg-white p-8 rounded-xl shadow-md hover:shadow-xl transition duration-300 border-b-4 border-transparent hover:border-brand-orange group">
                    <div class="bg-brand-light w-16 h-16 rounded-full flex items-center justify-center mb-6 group-hover:bg-brand-orange group-hover:text-white transition text-brand-blue">
                        <i data-lucide="map" class="w-8 h-8"></i>
                    </div>
                    <h3 class="font-heading font-bold text-xl mb-3 text-brand-blue">Strade e Opere Stradali</h3>
                    <p class="text-gray-600">Costruzione di strade montane, viabilità rurale, ripristino carreggiate, asfaltature e creazione di piazzali per il settore pubblico e privato.</p>
                </div>

                <!-- Servizio 5 -->
                <div class="bg-white p-8 rounded-xl shadow-md hover:shadow-xl transition duration-300 border-b-4 border-transparent hover:border-brand-orange group">
                    <div class="bg-brand-light w-16 h-16 rounded-full flex items-center justify-center mb-6 group-hover:bg-brand-orange group-hover:text-white transition text-brand-blue">
                        <i data-lucide="tree-pine" class="w-8 h-8"></i>
                    </div>
                    <h3 class="font-heading font-bold text-xl mb-3 text-brand-blue">Lavori Agrari e Forestali</h3>
                    <p class="text-gray-600">Gestione e manutenzione del patrimonio boschivo, pulizia terreni, disboscamento selettivo e riqualificazione ambientale con approccio sostenibile.</p>
                </div>

                <!-- Servizio 6 -->
                <div class="bg-white p-8 rounded-xl shadow-md hover:shadow-xl transition duration-300 border-b-4 border-transparent hover:border-brand-orange group">
                    <div class="bg-brand-light w-16 h-16 rounded-full flex items-center justify-center mb-6 group-hover:bg-brand-orange group-hover:text-white transition text-brand-blue">
                        <i data-lucide="building-2" class="w-8 h-8"></i>
                    </div>
                    <h3 class="font-heading font-bold text-xl mb-3 text-brand-blue">Realizzazione Fabbricati</h3>
                    <p class="text-gray-600">Costruzione e ristrutturazione di fabbricati artigianali, civili e industriali. Prepariamo l'area dalle fondamenta fino all'opera completa.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Instagram & Gallery Section -->
    <section id="instagram" class="py-20 bg-brand-blue text-white relative overflow-hidden">
        <div class="absolute inset-0 opacity-5">
            <div class="w-full h-full" style="background-image: url('data:image/svg+xml,%3Csvg width=\'60\' height=\'60\' viewBox=\'0 0 60 60\' xmlns=\'http://www.w3.org/2000/svg\'%3E%3Cg fill=\'none\' fill-rule=\'evenodd\'%3E%3Cg fill=\'#ffffff\' fill-opacity=\'1\'%3E%3Cpath d=\'M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z\'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E');"></div>
        </div>
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10 text-center">
            <div class="inline-flex items-center justify-center p-4 bg-gradient-to-tr from-orange-400 via-red-500 to-purple-500 rounded-full mb-6">
                <i data-lucide="instagram" class="w-12 h-12 text-white"></i>
            </div>
            <h2 class="font-heading font-800 text-3xl md:text-5xl mb-6">Il Nostro Impegno Quotidiano</h2>
            <div class="bg-white/10 p-8 rounded-2xl backdrop-blur-sm mb-10 border border-white/20 text-left">
                <p class="text-lg md:text-xl text-gray-200 mb-6 leading-relaxed">
                    Ogni giorno siamo sul campo per realizzare scavi, mettere in sicurezza i corsi d'acqua, costruire strade e prenderci cura delle aree boschive. Per noi di <strong>Alasonatti Scavi</strong>, ogni cantiere è una responsabilità: ci teniamo a consegnare opere sicure e ben fatte, risolvendo le problematiche dei nostri clienti con tempestività e competenza.
                </p>
                <p class="text-lg md:text-xl text-gray-200 leading-relaxed">
                    Vuoi vedere come lavoriamo e restare aggiornato sulle nostre attività? Sulla nostra pagina Instagram condividiamo costantemente le foto dei nostri cantieri, i dettagli degli interventi e la bellezza dei territori montani in cui abbiamo la fortuna di operare.
                </p>
            </div>

            <a href="https://instagram.com/alasonattiscavi" target="_blank" rel="noopener noreferrer" class="inline-flex bg-white text-brand-blue font-bold text-lg px-8 py-4 rounded-full hover:bg-gray-200 transition transform hover:-translate-y-1 shadow-lg items-center gap-3">
                <i data-lucide="instagram" class="w-6 h-6 text-brand-orange"></i> Vai alla Pagina Instagram
            </a>
        </div>
    </section>

    <!-- Contatti Section -->
    <section id="contatti" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-2 gap-16">
                
                <!-- Info Contatti -->
                <div>
                    <h2 class="font-heading font-800 text-3xl md:text-4xl text-brand-blue mb-6">Mettiamoci in Contatto</h2>
                    <div class="w-20 h-2 bg-brand-orange mb-8"></div>
                    <p class="text-gray-600 mb-10 text-lg">
                        Siamo a disposizione per consulenze, sopralluoghi gratuiti e preventivi per i tuoi progetti edili, forestali o stradali. Contattaci chiamando il nostro numero diretto.
                    </p>

                    <div class="space-y-6">
                        <div class="flex items-start gap-4 p-4 rounded-lg bg-brand-light border-l-4 border-brand-orange">
                            <div class="text-brand-orange">
                                <i data-lucide="map-pin" class="w-8 h-8"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-lg text-brand-blue">Sede Aziendale</h4>
                                <p class="text-gray-600">Fraz. Losa 4<br>10070 Pessinetto (TO)</p>
                            </div>
                        </div>

                        <div class="flex items-start gap-4 p-4 rounded-lg bg-brand-light border-l-4 border-brand-orange">
                            <div class="text-brand-orange">
                                <i data-lucide="phone" class="w-8 h-8"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-lg text-brand-blue">Telefono</h4>
                                <p class="text-gray-600 text-xl font-semibold">0123 504231</p>
                            </div>
                        </div>

                        <div class="flex items-start gap-4 p-4 rounded-lg bg-brand-light border-l-4 border-brand-orange">
                            <div class="text-brand-orange">
                                <i data-lucide="mail" class="w-8 h-8"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-lg text-brand-blue">Email</h4>
                                <p class="text-gray-600">info@alasonattiscavi.it</p>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Form Contatti (Ora abilitato per l'invio via email) -->
                <div class="bg-brand-blue p-8 rounded-xl shadow-lg border border-gray-200">
                    <h3 class="text-2xl font-bold text-white mb-6 font-heading">Inviaci un Messaggio</h3>
                    
                    <!-- Sostituisci info@alasonattiscavi.it con la tua email reale -->
                    <form action="https://formsubmit.co/info@alasonattiscavi.it" method="POST">
                        
                        <!-- Opzioni aggiuntive nascoste (Opzionali per togliere il captcha o cambiare pagina dopo l'invio) -->
                        <input type="hidden" name="_subject" value="Nuova richiesta dal sito web!">
                        <input type="hidden" name="_captcha" value="false">
                        
                        <div class="mb-4">
                            <label for="name" class="block text-sm font-semibold text-gray-200 mb-2">Nome e Cognome / Azienda</label>
                            <input type="text" id="name" name="nome" class="w-full px-4 py-3 rounded-md border-0 focus:outline-none focus:ring-2 focus:ring-brand-orange text-gray-800" required placeholder="Mario Rossi">
                        </div>
                        <div class="mb-4">
                            <label for="phone" class="block text-sm font-semibold text-gray-200 mb-2">Telefono</label>
                            <input type="tel" id="phone" name="telefono" class="w-full px-4 py-3 rounded-md border-0 focus:outline-none focus:ring-2 focus:ring-brand-orange text-gray-800" required placeholder="Il tuo recapito telefonico">
                        </div>
                        <div class="mb-6">
                            <label for="message" class="block text-sm font-semibold text-gray-200 mb-2">Descrivi la tua richiesta</label>
                            <textarea id="message" name="messaggio" rows="4" class="w-full px-4 py-3 rounded-md border-0 focus:outline-none focus:ring-2 focus:ring-brand-orange text-gray-800" required placeholder="Scrivi qui di cosa hai bisogno..."></textarea>
                        </div>
                        <button type="submit" class="w-full bg-brand-orange text-white font-bold py-4 rounded-md hover:bg-orange-500 transition flex justify-center items-center gap-2 shadow-md">
                            <i data-lucide="send" class="w-5 h-5"></i> Invia Richiesta
                        </button>
                    </form>
                </div>
                
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-brand-black text-gray-400 py-12 border-t border-gray-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Logo & Descrizione -->
                <div>
                    <div class="mb-4">
                        <img src="alasonatti logo compl copia 2.jpg" alt="Alasonatti Scavi Logo" class="h-16 w-auto object-contain">
                    </div>
                    <p class="text-sm mb-4 leading-relaxed">
                        Azienda a gestione familiare da 4 generazioni. Passione, professionalità e lavori fatti a regola d'arte nel settore edile, forestale e movimento terra a Pessinetto (TO).
                    </p>
                </div>
                
                <!-- Link Rapidi -->
                <div>
                    <h4 class="text-white font-bold mb-4 uppercase tracking-wider text-sm border-b border-gray-800 pb-2 inline-block">Link Rapidi</h4>
                    <ul class="space-y-2 text-sm">
                        <li><a href="#chi-siamo" class="hover:text-brand-orange transition flex items-center gap-2"><i data-lucide="chevron-right" class="w-4 h-4"></i> Chi Siamo</a></li>
                        <li><a href="#servizi" class="hover:text-brand-orange transition flex items-center gap-2"><i data-lucide="chevron-right" class="w-4 h-4"></i> Servizi Offerti</a></li>
                        <li><a href="#instagram" class="hover:text-brand-orange transition flex items-center gap-2"><i data-lucide="chevron-right" class="w-4 h-4"></i> Galleria Lavori</a></li>
                    </ul>
                </div>
                
                <!-- Social & Info -->
                <div>
                    <h4 class="text-white font-bold mb-4 uppercase tracking-wider text-sm border-b border-gray-800 pb-2 inline-block">Contatti & Info</h4>
                    <div class="space-y-2 text-sm mb-4">
                        <p><strong>Tel:</strong> 0123 504231</p>
                        <p><strong>Sede:</strong> Fraz. Losa 4, 10070 Pessinetto (TO)</p>
                    </div>
                    <div class="flex space-x-4 mb-4">
                        <a href="https://instagram.com/alasonattiscavi" target="_blank" class="w-10 h-10 rounded-full bg-gray-800 flex items-center justify-center hover:bg-brand-orange hover:text-white transition">
                            <i data-lucide="instagram" class="w-5 h-5"></i>
                        </a>
                        <a href="#" class="w-10 h-10 rounded-full bg-gray-800 flex items-center justify-center hover:bg-brand-orange hover:text-white transition">
                            <i data-lucide="facebook" class="w-5 h-5"></i>
                        </a>
                    </div>
                    <p class="text-xs text-gray-600">P.IVA: 04872310018</p>
                </div>
            </div>
            
            <div class="border-t border-gray-800 mt-12 pt-8 text-center text-sm">
                <p>&copy; 2026 Alasonatti Scavi. Tutti i diritti riservati.</p>
            </div>
        </div>
    </footer>

    <!-- Scripts -->
    <script>
        // Initialize Lucide Icons
        lucide.createIcons();

        // Mobile Menu Toggle
        const btn = document.getElementById('mobile-menu-btn');
        const menu = document.getElementById('mobile-menu');
        const mobileLinks = document.querySelectorAll('.mobile-link');

        btn.addEventListener('click', () => {
            menu.classList.toggle('hidden');
        });

        // Close mobile menu when clicking a link
        mobileLinks.forEach(link => {
            link.addEventListener('click', () => {
                menu.classList.add('hidden');
            });
        });

        // Navbar blur and color change on scroll
        window.addEventListener('scroll', () => {
            const nav = document.querySelector('nav');
            if (window.scrollY > 10) {
                nav.classList.add('shadow-lg');
                nav.classList.replace('bg-brand-black/95', 'bg-brand-black/100');
            } else {
                nav.classList.remove('shadow-lg');
                nav.classList.replace('bg-brand-black/100', 'bg-brand-black/95');
            }
        });
    </script>
</body>
</html>
