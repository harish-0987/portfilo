import { motion } from 'framer-motion'

export default function Portfolio() {
  return (
    <div className="min-h-screen bg-black text-white font-sans overflow-hidden">
      <div className="fixed inset-0 bg-[radial-gradient(circle_at_top_right,_rgba(59,130,246,0.15),transparent_30%),radial-gradient(circle_at_bottom_left,_rgba(168,85,247,0.15),transparent_30%)]"></div>
      {/* Hero Section */}
      <section className="relative flex flex-col items-center justify-center text-center px-6 py-32 bg-gradient-to-b from-black via-gray-900 to-black">
        <motion.div
          initial={{ opacity: 0, y: 40 }}
          animate={{ opacity: 1, y: 0 }}
          transition={{ duration: 1 }}
          className="absolute top-20 left-20 w-72 h-72 bg-cyan-500/20 rounded-full blur-3xl"
        />

        <motion.div
          initial={{ opacity: 0, y: -40 }}
          animate={{ opacity: 1, y: 0 }}
          transition={{ duration: 1 }}
          className="absolute bottom-10 right-20 w-72 h-72 bg-purple-500/20 rounded-full blur-3xl"
        />
        <motion.div
          initial={{ opacity: 0, scale: 0.9 }}
          animate={{ opacity: 1, scale: 1 }}
          transition={{ duration: 0.8 }}
          className="max-w-4xl relative z-10"
        >
          <div className="inline-flex items-center gap-3 px-5 py-2 rounded-full border border-cyan-500/30 bg-cyan-500/10 text-cyan-300 text-sm mb-8 backdrop-blur-xl shadow-lg">
            <span className="w-2 h-2 rounded-full bg-cyan-400 animate-pulse"></span>
            Available For AI/ML & Data Analytics Roles
          </div>

          <h1 className="text-6xl md:text-8xl font-extrabold mb-6 leading-tight bg-gradient-to-r from-cyan-300 via-white to-purple-400 bg-clip-text text-transparent">
            Pedda Pally Harish
          </h1>
          <p className="text-2xl md:text-3xl text-gray-200 mb-8 font-light tracking-wide">
            AI & ML Enthusiast | Data Analytics | Cloud Computing Learner
          </p>
          <p className="text-gray-300 text-xl leading-relaxed max-w-3xl mx-auto">
            Aspiring AI Engineer and Data Analyst passionate about Machine Learning, Cloud Computing, Python, and building intelligent solutions using modern technologies.
          </p>

          <div className="mt-12 flex flex-wrap gap-5 justify-center">
            <a
              href="mailto:peddapellyharish@gmail.com"
              className="group px-8 py-4 rounded-2xl bg-gradient-to-r from-cyan-500 to-blue-500 hover:scale-105 transition-all duration-300 font-semibold shadow-[0_0_40px_rgba(34,211,238,0.4)] flex items-center gap-2"
            >
              📧 Hire Me
            </a>

            <a
              href="https://www.linkedin.com/in/pedda-pally-harish-869180360"
              target="_blank"
              className="px-8 py-4 rounded-2xl border border-white/10 bg-white/5 backdrop-blur-xl hover:border-cyan-400 hover:scale-105 transition-all duration-300 shadow-xl"
            >
              <div className="flex items-center gap-2">🔗 LinkedIn</div>
            </a>
          </div>
                  <div className="mt-16 grid grid-cols-1 md:grid-cols-3 gap-8">
            <div className="group bg-white/5 backdrop-blur-2xl border border-white/10 rounded-[32px] p-8 shadow-[0_0_40px_rgba(255,255,255,0.05)] hover:scale-105 hover:border-cyan-400/40 transition-all duration-500">
              <div className="text-5xl mb-4">🤖</div>
              <h3 className="text-2xl font-bold mb-3">AI & ML</h3>
              <p className="text-gray-300 text-base leading-relaxed">Building intelligent solutions using machine learning and automation.</p>
            </div>

            <div className="group bg-white/5 backdrop-blur-2xl border border-white/10 rounded-[32px] p-8 shadow-[0_0_40px_rgba(255,255,255,0.05)] hover:scale-105 hover:border-cyan-400/40 transition-all duration-500">
              <div className="text-5xl mb-4">📊</div>
              <h3 className="text-2xl font-bold mb-3">Data Analytics</h3>
              <p className="text-gray-300 text-base leading-relaxed">Transforming raw data into actionable insights and visualizations.</p>
            </div>

            <div className="group bg-white/5 backdrop-blur-2xl border border-white/10 rounded-[32px] p-8 shadow-[0_0_40px_rgba(255,255,255,0.05)] hover:scale-105 hover:border-cyan-400/40 transition-all duration-500">
              <div className="text-5xl mb-4">☁️</div>
              <h3 className="text-2xl font-bold mb-3">Cloud Learning</h3>
              <p className="text-gray-300 text-base leading-relaxed">Exploring AWS cloud technologies and scalable architectures.</p>
            </div>
          </div>
        </motion.div>
      </section>

      {/* Skills */}
      <section className="relative px-6 py-24 max-w-6xl mx-auto">
        <h2 className="text-5xl font-extrabold mb-4 text-center bg-gradient-to-r from-cyan-300 to-purple-400 bg-clip-text text-transparent">Skills & Expertise</h2>
        <p className="text-center text-gray-400 max-w-2xl mx-auto mb-16 text-lg">Technologies and tools I use to create intelligent, scalable, and impactful solutions.</p>

        <div className="grid grid-cols-2 md:grid-cols-4 gap-6">
          {[
            'Python',
            'Machine Learning',
            'AI Automation',
            'Prompt Engineering',
            'SQL',
            'Power BI',
            'AWS',
            'Research Skills',
          ].map((skill) => (
            <div
              key={skill}
              className="group bg-gradient-to-b from-white/10 to-white/5 backdrop-blur-2xl border border-white/10 hover:border-cyan-400 transition-all duration-500 hover:-translate-y-3 hover:shadow-[0_0_40px_rgba(34,211,238,0.2)] rounded-[30px] p-8 text-center shadow-2xl"
            >
              <h3 className="text-xl font-bold tracking-wide">{skill}</h3>
            </div>
          ))}
        </div>
      </section>

      {/* Projects */}
      <section className="relative bg-gray-950/80 backdrop-blur-xl px-6 py-24">
        <div className="max-w-6xl mx-auto">
          <h2 className="text-5xl font-extrabold mb-4 text-center bg-gradient-to-r from-cyan-300 to-purple-400 bg-clip-text text-transparent">Featured Projects</h2>
          <p className="text-center text-gray-400 max-w-2xl mx-auto mb-16 text-lg">Real-world projects showcasing my skills in AI, Machine Learning, APIs, and intelligent systems.</p>

          <div className="grid md:grid-cols-2 gap-8">
            <div className="group relative overflow-hidden bg-gradient-to-b from-white/10 to-white/5 backdrop-blur-2xl border border-white/10 rounded-[34px] p-10 shadow-[0_0_40px_rgba(255,255,255,0.05)] hover:border-purple-500 hover:-translate-y-3 transition-all duration-500">
              <h3 className="text-2xl font-bold mb-4 text-cyan-400">
                Healthcare Diagnostic System
              </h3>
              <p className="text-gray-400 leading-relaxed">
                Built a machine learning based healthcare diagnostic system capable of predicting diseases using patient data and intelligent algorithms.
              </p>
            </div>

            <div className="group relative overflow-hidden bg-gradient-to-b from-white/10 to-white/5 backdrop-blur-2xl border border-white/10 rounded-[34px] p-10 shadow-[0_0_40px_rgba(255,255,255,0.05)] hover:border-purple-500 hover:-translate-y-3 transition-all duration-500">
              <h3 className="text-2xl font-bold mb-4 text-cyan-400">
                Travel Itinerary Planner
              </h3>
              <p className="text-gray-400 leading-relaxed">
                Developed a smart travel itinerary planner integrating APIs for route optimization, recommendations, and real-time travel planning.
              </p>
            </div>
          </div>
        </div>
      </section>

      {/* Certifications */}
      <section className="relative px-6 py-24 max-w-5xl mx-auto">
        <h2 className="text-5xl font-extrabold mb-4 text-center bg-gradient-to-r from-cyan-300 to-purple-400 bg-clip-text text-transparent">Certifications</h2>
        <p className="text-center text-gray-400 max-w-2xl mx-auto mb-16 text-lg">Continuous learning through certifications and workshops in AI, Cloud, and Analytics.</p>

        <div className="grid md:grid-cols-2 gap-6">
          {[
            'AWS Certifications',
            'Generative AI',
            'AI for Beginners',
            'Power BI Workshop',
            '5 Days Full Stack Workshop',
          ].map((cert) => (
            <div
              key={cert}
              className="bg-white/5 backdrop-blur-xl border border-white/10 rounded-3xl p-6 hover:border-cyan-400 hover:-translate-y-1 transition-all duration-300"
            >
              <p className="text-lg">{cert}</p>
            </div>
          ))}
        </div>
      </section>

      {/* Education */}
      <section className="relative bg-gray-950/80 backdrop-blur-xl px-6 py-24">
        <div className="max-w-5xl mx-auto">
          <h2 className="text-5xl font-extrabold mb-4 text-center bg-gradient-to-r from-cyan-300 to-purple-400 bg-clip-text text-transparent">Education</h2>
          <p className="text-center text-gray-400 max-w-2xl mx-auto mb-16 text-lg">My academic journey focused on Computer Science, AI technologies, and modern software development.</p>

          <div className="space-y-6">
            <div className="bg-white/5 backdrop-blur-2xl rounded-[30px] p-8 border border-white/10 hover:border-cyan-400 transition-all duration-500 hover:-translate-y-2 shadow-2xl">
              <h3 className="text-2xl font-semibold text-cyan-400">
                Vaagdevi College of Engineering
              </h3>
              <p className="text-gray-400 mt-2">
                B.Tech in Computer Science Engineering • 2025
              </p>
            </div>

            <div className="bg-white/5 backdrop-blur-2xl rounded-[30px] p-8 border border-white/10 hover:border-cyan-400 transition-all duration-500 hover:-translate-y-2 shadow-2xl">
              <h3 className="text-2xl font-semibold text-cyan-400">
                SVS Group of Institutions
              </h3>
              <p className="text-gray-400 mt-2">
                Diploma in Computer Science • 2020 - 2023
              </p>
            </div>
          </div>
        </div>
      </section>

      {/* Contact */}
      <section className="relative px-6 py-28 text-center">
        <h2 className="text-6xl font-extrabold mb-6 bg-gradient-to-r from-cyan-300 to-purple-400 bg-clip-text text-transparent">Let's Build Something Amazing</h2>

        <p className="text-gray-400 text-lg mb-8">
          Open for internships, full-time roles, freelance opportunities, and exciting collaborations in AI/ML, Data Analytics, and Cloud Computing.
        </p>

        <div className="flex flex-col md:flex-row gap-4 justify-center items-center mb-10">
          <a
            href="mailto:peddapellyharish@gmail.com"
            className="px-10 py-5 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-2xl font-semibold hover:scale-105 transition-all duration-300 shadow-[0_0_40px_rgba(34,211,238,0.35)]"
          >
            <div className="flex items-center gap-2">📧 Email Me</div>
          </a>

          <a
            href="tel:+917993871365"
            className="px-10 py-5 border border-white/10 bg-white/5 backdrop-blur-xl rounded-2xl hover:border-cyan-400 hover:scale-105 transition-all duration-300 shadow-2xl"
          >
            <div className="flex items-center gap-2">📱 Call Me</div>
          </a>
        </div>
              <div className="flex justify-center gap-6 mt-8">
          <a href="https://github.com" target="_blank" className="p-4 rounded-full bg-white/5 border border-white/10 hover:border-cyan-400 transition-all duration-300 hover:scale-110">
            <span className="text-xl">💻</span>
          </a>

          <a href="https://www.linkedin.com/in/pedda-pally-harish-869180360" target="_blank" className="p-4 rounded-full bg-white/5 border border-white/10 hover:border-cyan-400 transition-all duration-300 hover:scale-110">
            <span className="text-xl">🔗</span>
          </a>

          <a href="mailto:peddapellyharish@gmail.com" className="p-4 rounded-full bg-white/5 border border-white/10 hover:border-cyan-400 transition-all duration-300 hover:scale-110">
            <span className="text-xl">📧</span>
          </a>
        </div>
      </section>
    </div>
  )
}
