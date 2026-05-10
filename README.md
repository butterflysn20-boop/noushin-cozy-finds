# noushin-cozy-finds
export default function NoushinCozyFinds() {
  const products = [
    {
      title: "Cozy Desk Setup",
      desc: "Cute & aesthetic desk accessories ✨",
      link: "#",
      image:
        "https://images.unsplash.com/photo-1516321318423-f06f85e504b3?q=80&w=1200&auto=format&fit=crop",
    },
    {
      title: "Beauty Essentials",
      desc: "Soft girl skincare & beauty finds 💄",
      link: "#",
      image:
        "https://images.unsplash.com/photo-1522335789203-aabd1fc54bc9?q=80&w=1200&auto=format&fit=crop",
    },
    {
      title: "Cute Gadgets",
      desc: "Amazon finds you’ll love 🤍",
      link: "#",
      image:
        "https://images.unsplash.com/photo-1517336714739-489689fd1ca8?q=80&w=1200&auto=format&fit=crop",
    },
  ];

  return (
    <div className="min-h-screen bg-[#fdf8f5] text-gray-800 overflow-hidden">
      {/* HERO SECTION */}
      <div className="max-w-6xl mx-auto px-6 py-12">
        <div className="text-center mb-16">
          <p className="uppercase tracking-[0.35em] text-sm text-[#9f8578] mb-4">
            Pinterest Inspired Affiliate Finds
          </p>

          <h1 className="text-5xl md:text-7xl font-serif font-semibold text-[#6d4c41] mb-6 leading-tight">
            Noushin’s
            <br />
            Cozy Finds ☁️
          </h1>

          <p className="max-w-2xl mx-auto text-lg text-gray-600 leading-relaxed">
            Handpicked cozy finds, dreamy lifestyle products, beauty
            favorites & aesthetic Amazon discoveries curated by Noushin ✨
          </p>

          <div className="mt-8 flex justify-center gap-4 flex-wrap">
            <a
              href="#"
              className="px-7 py-3 rounded-full bg-[#e8d8d0] hover:bg-[#dcc7bd] hover:scale-105 transition duration-300 text-[#5d4037] font-medium shadow-md"
            >
              Shop My Finds
            </a>

            <a
              href="#"
              className="px-7 py-3 rounded-full bg-white hover:scale-105 transition duration-300 text-[#5d4037] font-medium shadow-md"
            >
              Pinterest
            </a>
          </div>
        </div>

        {/* PRODUCT GRID */}
        <div className="grid md:grid-cols-3 gap-8">
          {products.map((product, index) => (
            <div
              key={index}
              className="bg-white rounded-[32px] overflow-hidden shadow-xl hover:-translate-y-2 hover:shadow-2xl transition duration-300"
            >
              <div className="overflow-hidden">
                <img
                  src={product.image}
                  alt={product.title}
                  className="h-72 w-full object-cover hover:scale-110 transition duration-500"
                />
              </div>

              <div className="p-6">
                <h2 className="text-2xl font-semibold mb-3 text-[#5d4037]">
                  {product.title}
                </h2>

                <p className="text-gray-600 mb-6 leading-relaxed">
                  {product.desc}
                </p>

                <a
                  href={product.link}
                  className="inline-block px-5 py-3 rounded-full bg-[#f3e7e1] hover:bg-[#e6d4ca] hover:scale-105 transition duration-300 text-[#5d4037] font-medium"
                >
                  Shop Now ✨
                </a>
              </div>
            </div>
          ))}
        </div>

        {/* ABOUT SECTION */}
        <div className="mt-24 bg-white rounded-[40px] p-10 md:p-14 shadow-xl text-center">
          <h3 className="text-4xl font-serif text-[#6d4c41] mb-5">
            About Noushin 🤍
          </h3>

          <p className="max-w-3xl mx-auto text-gray-600 leading-relaxed text-lg">
            Welcome to my cozy little corner of the internet ☁️
            Here I share dreamy Amazon finds, cute room decor,
            beauty favorites, aesthetic lifestyle products & Pinterest-inspired
            discoveries that make everyday life feel softer and prettier ✨
          </p>
        </div>

        {/* SOCIAL SECTION */}
        <div className="mt-20 text-center">
          <h3 className="text-4xl font-serif mb-5 text-[#6d4c41]">
            Follow Noushin ☁️
          </h3>

          <p className="text-gray-600 mb-8 text-lg">
            Pinterest • Amazon Finds • Cozy Lifestyle • Aesthetic Content
          </p>

          <div className="flex justify-center gap-5 flex-wrap">
            <a
              href="#"
              className="px-7 py-3 rounded-full bg-white shadow-lg hover:shadow-2xl hover:-translate-y-1 transition duration-300"
            >
              Pinterest
            </a>

            <a
              href="#"
              className="px-7 py-3 rounded-full bg-white shadow-lg hover:shadow-2xl hover:-translate-y-1 transition duration-300"
            >
              Amazon Storefront
            </a>

            <a
              href="#"
              className="px-7 py-3 rounded-full bg-white shadow-lg hover:shadow-2xl hover:-translate-y-1 transition duration-300"
            >
              TikTok
            </a>

            <a
              href="#"
              className="px-7 py-3 rounded-full bg-white shadow-lg hover:shadow-2xl hover:-translate-y-1 transition duration-300"
            >
              Instagram
            </a>
          </div>

          <p className="text-xs text-gray-400 mt-10">
            As an Amazon Associate, I earn from qualifying purchases 🤍
          </p>
        </div>
      </div>
    </div>
  );
}
