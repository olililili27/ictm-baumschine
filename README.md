# ictm-baumschine
export default function Page() {
  return (
    <div className="min-h-screen w-full bg-gray-100 text-slate-800">
      {/* Top contact bar */}
      <div className="w-full bg-slate-800 text-white text-sm hidden md:block">
        <div className="max-w-6xl mx-auto flex items-center justify-end gap-6 py-2 px-4">
          <a href="mailto:info@ictm-baumaschinen.de" className="hover:underline">info@ictm-baumaschinen.de</a>
          <a href="tel:+4968139689991" className="hover:underline">+49 681 39689991</a>
          <a href="tel:+4917624670229" className="hover:underline">+49 176 24670229</a>
        </div>
      </div>

      {/* Header */}
      <header className="w-full bg-white shadow-sm">
        <div className="max-w-6xl mx-auto flex items-center justify-between py-4 px-4">
          {/* Logo */}
          <div className="flex items-center gap-3">
            <div className="h-8 w-10 rounded-sm bg-gradient-to-br from-yellow-400 to-amber-600 flex items-center justify-center">
              <svg viewBox="0 0 64 64" className="h-6 w-6 text-slate-900" fill="currentColor" aria-hidden>
                <path d="M8 42h6l4-8h8l6 8h8l-8-12 6-8h6l8 10-2 2-4-5-3 4 5 7v4h-6v-2H14v2H8v-2l2-2z" />
              </svg>
            </div>
            <div className="leading-tight">
              <div className="font-semibold text-slate-900 text-lg">ICTM Baumaschinen</div>
              <div className="text-xs tracking-wide text-slate-500 -mt-1">Verkauf – Ankauf – Vermietung – Service</div>
            </div>
          </div>

          {/* Nav */}
          <nav className="hidden md:flex items-center gap-6 text-slate-700">
            {[
              ["Startseite", "#startseite"],
              ["Über uns", "#ueber-uns"],
              ["Fahrzeuge", "#fahrzeuge"],
              ["Ankauf", "#ankauf"],
              ["Vermietung", "#vermietung"],
              ["Service", "#service"],
              ["Kontakt", "#kontakt"],
            ].map(([label, href]) => (
              <a key={href} href={href} className="hover:text-slate-900">{label}</a>
            ))}
          </nav>
        </div>
      </header>

      {/* Hero */}
      <section id="startseite" className="bg-slate-900">
        <div className="max-w-6xl mx-auto grid md:grid-cols-2 gap-8 items-center px-4 py-16">
          <div className="text-white">
            <h1 className="text-3xl md:text-4xl font-extrabold leading-tight">
              Verkauf – Ankauf – Vermietung – Service
            </h1>
            <p className="mt-4 text-slate-300 max-w-prose">
              Willkommen bei ICTM Baumaschinen – Ihrem zuverlässigen Partner für gebrauchte Baumaschinen und Nutzfahrzeuge in Saarbrücken und ganz Deutschland.
              Wir kaufen, verkaufen und vermieten hochwertige Maschinen aus eigenem Bestand. Unsere Fahrzeuge sind geprüft, gepflegt und sofort einsatzbereit.
            </p>
            <p className="mt-4 text-slate-300">👉 Entdecken Sie unser aktuelles Angebot oder kontaktieren Sie uns für individuelle Anfragen.</p>
          </div>

          {/* Hero image placeholder */}
          <div
            className="relative h-56 md:h-72 lg:h-80 rounded-lg shadow-lg bg-cover bg-center"
            style={{ backgroundImage: "url('/images/hero-excavator.png')" }}
            aria-label="Bagger auf Baustelle"
          >
            <div className="absolute inset-0 bg-gradient-to-tr from-slate-900/40 to-transparent rounded-lg" />
          </div>
        </div>
      </section>

      {/* Über uns */}
      <section id="ueber-uns" className="bg-white py-12">
        <div className="max-w-6xl mx-auto px-4">
          <h2 className="text-2xl font-bold mb-4">Über die Firma ICTM Baumaschinen</h2>
          <p className="text-slate-700 leading-relaxed">
            Die Firma ICTM Baumaschinen steht für Qualität, Zuverlässigkeit und faire Preise. Mit langjähriger Erfahrung im Bereich Baumaschinen und Nutzfahrzeuge bieten wir unseren Kunden einen umfassenden Service – vom Ankauf über die Vermietung bis hin zum Verkauf.
          </p>
          <p className="mt-3 text-slate-700 leading-relaxed">
            Unsere Maschinen stammen ausschließlich aus unserem eigenen Bestand oder von ausgewählten Partnern. Wir legen großen Wert auf Transparenz, technische Prüfung und Kundenzufriedenheit.
          </p>
        </div>
      </section>

      {/* Fahrzeuge */}
      <section id="fahrzeuge" className="bg-gray-50 py-12">
        <div className="max-w-6xl mx-auto px-4">
          <h2 className="text-2xl font-bold mb-4">Fahrzeuge / Maschinen (Angebote)</h2>
          <p className="text-slate-700 mb-4">In unserem Sortiment finden Sie:</p>
          <ul className="list-disc list-inside space-y-1 text-slate-700">
            <li>Bagger</li>
            <li>Radlader</li>
            <li>Walzen</li>
            <li>Dumper</li>
            <li>LKW und Transportfahrzeuge</li>
            <li>Gabelstapler</li>
            <li>u.v.m.</li>
          </ul>
          <p className="mt-4 text-slate-700">Alle Maschinen sind sofort verfügbar und können auf Anfrage besichtigt werden.</p>
          <p className="mt-2 text-slate-700">➡️ Kontaktieren Sie uns für aktuelle Angebote oder senden Sie uns Ihre Wunschliste!</p>
        </div>
      </section>

      {/* Ankauf */}
      <section id="ankauf" className="bg-white py-12">
        <div className="max-w-6xl mx-auto px-4">
          <h2 className="text-2xl font-bold mb-4">Ankauf (Wir kaufen Ihre Maschinen)</h2>
          <p className="text-slate-700 leading-relaxed">
            Sie möchten Ihre gebrauchte Baumaschine oder Ihr Nutzfahrzeug verkaufen? Wir kaufen zuverlässig und unkompliziert – zu fairen Preisen.
          </p>
          <p className="mt-2 text-slate-700 leading-relaxed">
            Einfach anrufen oder eine E-Mail mit Fotos und technischen Daten senden. Wir machen Ihnen ein unverbindliches Angebot!
          </p>
          <p className="mt-4 text-slate-700">
            📧 <a href="mailto:info@ictm-baumaschinen.de" className="text-sky-700 hover:underline">info@ictm-baumaschinen.de</a><br />
            📞 +49 681 39689991
          </p>
        </div>
      </section>

      {/* Vermietung */}
      <section id="vermietung" className="bg-gray-50 py-12">
        <div className="max-w-6xl mx-auto px-4">
          <h2 className="text-2xl font-bold mb-4">Vermietung (Maschinen mieten)</h2>
          <p className="text-slate-700 leading-relaxed">
            Benötigen Sie eine Maschine nur für einen bestimmten Zeitraum? Kein Problem – bei uns können Sie viele Modelle kurz- oder langfristig mieten.
          </p>
          <p className="mt-2 text-slate-700 leading-relaxed">
            Wir beraten Sie gerne bei der Auswahl der passenden Maschine für Ihr Projekt.
          </p>
        </div>
      </section>

      {/* Service */}
      <section id="service" className="bg-white py-12">
        <div className="max-w-6xl mx-auto px-4">
          <h2 className="text-2xl font-bold mb-4">Service (Wartung und Beratung)</h2>
          <p className="text-slate-700 leading-relaxed">
            Unser Service endet nicht beim Verkauf. Wir unterstützen Sie auch nach dem Kauf mit:
          </p>
          <ul className="list-disc list-inside mt-3 space-y-1 text-slate-700">
            <li>Wartung und Pflege</li>
            <li>Ersatzteilen</li>
            <li>Technischer Beratung</li>
          </ul>
          <p className="mt-4 text-slate-700">Ihre Zufriedenheit ist unser Ziel.</p>
        </div>
      </section>

      {/* Kontakt */}
      <section id="kontakt" className="bg-gray-50 py-12">
        <div className="max-w-6xl mx-auto px-4">
          <h2 className="text-2xl font-bold mb-4">Kontakt</h2>
          <p className="text-slate-700 leading-relaxed">
            📍 ICTM Baumaschinen<br />
            Lebacher Straße 145<br />
            66113 Saarbrücken, Deutschland
          </p>
          <p className="mt-3 text-slate-700 leading-relaxed">
            📧 <a href="mailto:info@ictm-baumaschinen.de" className="text-sky-700 hover:underline">info@ictm-baumaschinen.de</a><br />
            📞 0049 681 39689991<br />
            📱 0049 176 24670229
          </p>
          <p className="mt-4 text-slate-700">Oder nutzen Sie einfach unser Kontaktformular – wir melden uns schnellstmöglich bei Ihnen.</p>
        </div>
      </section>

      {/* Footer */}
      <footer className="bg-white border-t mt-10">
        <div className="max-w-6xl mx-auto px-4 py-8 text-sm text-slate-600 flex flex-col md:flex-row items-center justify-between gap-4">
          <div>© {new Date().getFullYear()} ICTM Baumaschinen</div>
          <div className="flex items-center gap-6">
            <a href="#impressum" className="hover:underline">Impressum</a>
            <a href="#datenschutz" className="hover:underline">Datenschutz</a>
            <a href="#kontakt" className="hover:underline">Kontakt</a>
          </div>
        </div>
      </footer>
    </div>
  );
}
