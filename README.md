import React from 'react';
import { Github, Linkedin, Twitter, Mail } from 'lucide-react';

const ProfileHeader = () => {
  return (
    <div className="w-full bg-gradient-to-r from-gray-900 to-blue-900 p-8 rounded-lg shadow-2xl">
      {/* Main Title */}
      <div className="text-center mb-8">
        <h1 className="text-4xl font-bold bg-clip-text text-transparent bg-gradient-to-r from-blue-400 to-purple-600 mb-4">
          🌟 NEURAL MATRIX ARSENAL 🌟
        </h1>
        <h2 className="text-2xl text-blue-300 font-semibold">Rohit Vyavahare</h2>
        <div className="text-blue-400 mt-2 space-x-2">
          <span>Data Science</span> • 
          <span>AI</span> • 
          <span>Machine Learning</span> • 
          <span>Deep Learning</span> • 
          <span>NLP</span> • 
          <span>Generative AI</span>
        </div>
      </div>

      {/* Tech Stack Grid */}
      <div className="grid grid-cols-6 gap-4 mb-8">
        {[
          'Python', 'SQL', 'Jupyter', 'Flask', 'FastAPI', 'Matplotlib',
          'Seaborn', 'Pandas', 'NumPy', 'Scikit-learn', 'PyTorch', 'TensorFlow',
          'GPT', 'Llama', 'Langchain', 'VS Code', 'GitHub', 'React'
        ].map((tech) => (
          <div key={tech} className="bg-gray-800 p-3 rounded-lg text-center hover:bg-gray-700 transition-colors">
            <div className="text-blue-400 font-semibold">{tech}</div>
          </div>
        ))}
      </div>

      {/* Code Block */}
      <div className="bg-gray-800 p-4 rounded-lg mb-8 font-mono text-sm text-blue-300">
        <pre>
{`model.compile(
    life = "Coding",
    passion = "AI",
    mission = "Innovation"
)

while alive:
    eat()
    sleep()
    code()
    repeat()`}
        </pre>
      </div>

      {/* Timeline */}
      <div className="bg-gray-800 p-4 rounded-lg mb-8">
        <h3 className="text-2xl font-bold text-blue-400 mb-4">⚡ INNOVATION TIMELINE ⚡</h3>
        <div className="space-y-4">
          {[
            { year: '2022', desc: 'Explored AI/ML, mastered Python & SQL fundamentals' },
            { year: '2023', desc: 'Deep dived into Machine Learning, Deep Learning & NLP' },
            { year: '2024', desc: 'Mastered Generative AI & Large Language Models' },
            { year: '2025', desc: 'Advancing into AI Agents & Autonomous Systems' }
          ].map(({ year, desc }) => (
            <div key={year} className="flex items-center space-x-4">
              <div className="text-purple-400 font-bold w-16">{year}</div>
              <div className="flex-1 bg-gray-700 p-2 rounded">{desc}</div>
            </div>
          ))}
        </div>
      </div>

      {/* Social Links */}
      <div className="flex justify-center space-x-6">
        <a href="https://www.linkedin.com/in/rohitvyavahare2001" className="text-blue-400 hover:text-blue-300">
          <Linkedin className="w-6 h-6" />
        </a>
        <a href="https://x.com/RV_vyavahare" className="text-blue-400 hover:text-blue-300">
          <Twitter className="w-6 h-6" />
        </a>
        <a href="mailto:rohitvyavahare2001@gmail.com" className="text-blue-400 hover:text-blue-300">
          <Mail className="w-6 h-6" />
        </a>
        <a href="https://github.com" className="text-blue-400 hover:text-blue-300">
          <Github className="w-6 h-6" />
        </a>
      </div>
    </div>
  );
};

export default ProfileHeader;
