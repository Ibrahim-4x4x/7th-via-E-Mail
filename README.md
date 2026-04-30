<!--DOCTYPE html-->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Unit 7: Communication Interactive Activities</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body { background-color: #f0f4f8; font-family: 'Segoe UI', sans-serif; }
        .quiz-card { background: white; border-radius: 1.5rem; box-shadow: 0 10px 25px rgba(0,0,0,0.1); }
        .hidden { display: none; }
    </style>
</head>
<body class="p-4 md:p-8">

<div class="max-w-4xl mx-auto quiz-card p-6 md:p-10">
    <div id="start-screen" class="text-center py-10">
        <div class="mb-6 inline-block p-4 bg-blue-100 rounded-full">
            <svg class="w-12 h-12 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 12h.01M12 12h.01M16 12h.01M21 12c0 4.418-4.03 8-9 8a9.863 9.863 0 01-4.255-.949L3 20l1.395-3.72C3.512 15.042 3 13.574 3 12c0-4.418 4.03-8 9-8s9 3.582 9 8z"></path></svg>
        </div>
        <h1 class="text-4xl font-bold text-blue-900 mb-2">Unit 7: Let's Talk!</h1>
        <p class="text-gray-600 mb-8 text-lg">Communication & Technology Activities</p>
        
        <div class="space-y-4 max-w-md mx-auto bg-gray-50 p-6 rounded-2xl border border-gray-200">
            <input type="text" id="student-name" class="w-full p-3 border rounded-lg outline-none focus:ring-2 focus:ring-blue-400" placeholder="Student Full Name">
            <input type="email" id="teacher-email" class="w-full p-3 border rounded-lg outline-none focus:ring-2 focus:ring-red-400" placeholder="Teacher's Email Address">
            <button onclick="initQuiz()" class="w-full bg-blue-600 text-white py-4 rounded-xl font-bold hover:bg-blue-700 transition transform hover:scale-105 shadow-lg">Start Activity</button>
        </div>
        <p class="text-xs text-gray-400 mt-6">* Note: You can only submit your answers once.</p>
    </div>

    <div id="quiz-screen" class="hidden">
        <div class="flex justify-between items-center mb-8 sticky top-0 bg-white/90 backdrop-blur-sm py-4 border-b z-10">
            <span class="font-bold text-blue-700" id="display-name"></span>
            <span class="bg-blue-600 text-white px-4 py-2 rounded-full text-sm font-bold">Unit 7 Quiz</span>
        </div>

        <form id="quiz-form">
            <div class="mb-12">
                <h2 class="text-2xl font-black text-blue-800 mb-6 flex items-center">Lesson 1: Vocabulary</h2>
                <div class="grid md:grid-cols-2 gap-6">
                    <div class="p-4 bg-gray-50 rounded-xl">
                        <p class="font-medium mb-3">1. I'm going to ______ to a podcast. [cite: 8]</p>
                        <select name="l1_q1" class="w-full p-2 border rounded">
                            <option value="">Select...</option>
                            <option value="insert">insert</option>
                            <option value="listen">listen</option>
                            <option value="use">use</option>
                        </select>
                    </div>
                    <div class="p-4 bg-gray-50 rounded-xl">
                        <p class="font-medium mb-3">2. Lisa likes to ______ to friends online. [cite: 9]</p>
                        <select name="l1_q2" class="w-full p-2 border rounded">
                            <option value="">Select...</option>
                            <option value="chat">chat</option>
                            <option value="receive">receive</option>
                            <option value="get">get</option>
                        </select>
                    </div>
                    <div class="p-4 bg-gray-50 rounded-xl">
                        <p class="font-medium mb-3">3. Dad doesn't like ______ social media. [cite: 10]</p>
                        <select name="l1_q3" class="w-full p-2 border rounded">
                            <option value="">Select...</option>
                            <option value="writing">writing</option>
                            <option value="using">using</option>
                            <option value="seeing">seeing</option>
                        </select>
                    </div>
                    <div class="p-4 bg-gray-50 rounded-xl">
                        <p class="font-medium mb-3">4. We'd like to ______ a vlog about UAE. [cite: 11]</p>
                        <select name="l1_q4" class="w-full p-2 border rounded">
                            <option value="">Select...</option>
                            <option value="watch">watch</option>
                            <option value="get">get</option>
                            <option value="use">use</option>
                        </select>
                    </div>
                </div>
            </div>

            <div class="mb-12">
                <h2 class="text-2xl font-black text-blue-800 mb-6">Survey Questions</h2>
                <div class="space-y-4">
                    <div class="p-3 bg-white border rounded-lg">
                        <p class="mb-2">Q: Do you often <span class="text-blue-600 font-mono">[ceevrie xett samsegse]</span>? [cite: 23]</p>
                        <input type="text" name="u1" class="w-full border-b-2 border-blue-200 p-1" placeholder="Unscramble here...">
                    </div>
                    <div class="p-3 bg-white border rounded-lg">
                        <p class="mb-2">Q: Could you <span class="text-blue-600 font-mono">[pkee a creste]</span> if told one? [cite: 24]</p>
                        <input type="text" name="u2" class="w-full border-b-2 border-blue-200 p-1" placeholder="Unscramble here...">
                    </div>
                    <div class="p-3 bg-white border rounded-lg">
                        <p class="mb-2">Q: Do you usually <span class="text-blue-600 font-mono">[itle eth utthr]</span> to friends? [cite: 25]</p>
                        <input type="text" name="u3" class="w-full border-b-2 border-blue-200 p-1" placeholder="Unscramble here...">
                    </div>
                </div>
            </div>

            <div class="mb-12">
                <h2 class="text-2xl font-black text-blue-800 mb-6">Opposites</h2>
                <div class="bg-indigo-50 p-6 rounded-2xl border border-indigo-100 space-y-4">
                    <p>1. If you can't keep a secret, people won't <input type="text" name="opp1" class="w-24 border-b border-indigo-400 bg-transparent text-center"> you any. [cite: 29]</p>
                    <p>2. I can't receive or <input type="text" name="opp2" class="w-24 border-b border-indigo-400 bg-transparent text-center"> a text message. [cite: 31]</p>
                    <p>3. You shouldn't tell lies, you should always tell the <input type="text" name="opp3" class="w-24 border-b border-indigo-400 bg-transparent text-center">. [cite: 37]</p>
                    <p>4. You should try to <input type="text" name="opp4" class="w-24 border-b border-indigo-400 bg-transparent text-center"> a promise. [cite: 40]</p>
                </div>
            </div>

            <div class="mb-12">
                <h2 class="text-2xl font-black text-blue-800 mb-6">Lesson 2: Dialogue</h2>
                <div class="space-y-4 text-gray-700 italic">
                    <p>1. I'm <input type="text" name="d1" class="border-b border-gray-400 w-24 text-center"> to get on well for a month. [cite: 48]</p>
                    <p>2. I haven't had any <input type="text" name="d2" class="border-b border-gray-400 w-24 text-center"> with them. [cite: 50]</p>
                    <p>3. I was so angry and we had a <input type="text" name="d3" class="border-b border-gray-400 w-24 text-center"> argument! [cite: 54]</p>
                    <p>4. I think <input type="text" name="d4" class="border-b border-gray-400 w-24 text-center"> will be as popular as vlogs. [cite: 60]</p>
                </div>
            </div>

            <div class="mb-12">
                <h2 class="text-2xl font-black text-blue-800 mb-6">Comprehension</h2>
                <div class="space-y-4">
                    <div class="flex justify-between items-center p-3 bg-gray-50 rounded-lg">
                        <span>1. Dana has been doing an experiment for a week. [cite: 66]</span>
                        <div class="space-x-4">
                            <label><input type="radio" name="tf1" value="T"> T</label>
                            <label><input type="radio" name="tf1" value="F"> F</label>
                        </div>
                    </div>
                    <div class="flex justify-between items-center p-3 bg-gray-50 rounded-lg">
                        <span>2. Dana gets on worse with her sister than friends. [cite: 68]</span>
                        <div class="space-x-4">
                            <label><input type="radio" name="tf2" value="T"> T</label>
                            <label><input type="radio" name="tf2" value="F"> F</label>
                        </div>
                    </div>
                </div>
            </div>

            <button type="button" onclick="submitToEmail()" class="w-full bg-red-600 text-white py-5 rounded-2xl font-bold text-2xl hover:bg-red-700 transition shadow-xl">Submit All Results</button>
        </form>
    </div>

    <div id="finish-screen" class="hidden text-center py-20">
        <div class="text-8xl mb-6">✅</div>
        <h2 class="text-4xl font-bold text-gray-800 mb-4">Quiz Finished!</h2>
        <p id="score-display" class="text-5xl text-blue-600 font-black mb-6"></p>
        <p class="text-gray-500">Your results have been sent to your teacher. You cannot retake this quiz.</p>
    </div>
</div>

<script>
    const STORAGE_KEY = 'unit7_quiz_lock';

    window.onload = () => {
        const savedScore = localStorage.getItem(STORAGE_KEY);
        if (savedScore) {
            showFinish(savedScore);
        }
    };

    function initQuiz() {
        const name = document.getElementById('student-name').value;
        const email = document.getElementById('teacher-email').value;
        
        if (!name.trim() || !email.trim()) {
            alert("Please enter your name and teacher's email!");
            return;
        }

        document.getElementById('start-screen').classList.add('hidden');
        document.getElementById('quiz-screen').classList.remove('hidden');
        document.getElementById('display-name').innerText = "Student: " + name;
        window.scrollTo(0,0);
    }

    function showFinish(score) {
        document.getElementById('start-screen').classList.add('hidden');
        document.getElementById('quiz-screen').classList.add('hidden');
        document.getElementById('finish-screen').classList.remove('hidden');
        document.getElementById('score-display').innerText = `Score: ${score} / 17`;
    }

    function calculateScore() {
        const data = new FormData(document.getElementById('quiz-form'));
        let score = 0;
        
        // Keys: listen, chat, using, watch, receive text messages, keep a secret, tell the truth, tell, send, truth, keep, trying, arguments, huge, podcasts, F, T
        if (data.get('l1_q1') === 'listen') score++;
        if (data.get('l1_q2') === 'chat') score++;
        if (data.get('l1_q3') === 'using') score++;
        if (data.get('l1_q4') === 'watch') score++;
        if (data.get('u1')?.toLowerCase().trim() === 'receive text messages') score++;
        if (data.get('u2')?.toLowerCase().trim() === 'keep a secret') score++;
        if (data.get('u3')?.toLowerCase().trim() === 'tell the truth') score++;
        if (data.get('opp1')?.toLowerCase().trim() === 'tell') score++;
        if (data.get('opp2')?.toLowerCase().trim() === 'send') score++;
        if (data.get('opp3')?.toLowerCase().trim() === 'truth') score++;
        if (data.get('opp4')?.toLowerCase().trim() === 'keep') score++;
        if (data.get('d1')?.toLowerCase().trim() === 'trying') score++;
        if (data.get('d2')?.toLowerCase().trim() === 'arguments') score++;
        if (data.get('d3')?.toLowerCase().trim() === 'huge') score++;
        if (data.get('d4')?.toLowerCase().trim() === 'podcasts') score++;
        if (data.get('tf1') === 'F') score++;
        if (data.get('tf2') === 'T') score++;
        
        return score;
    }

    function submitToEmail() {
        const score = calculateScore();
        const name = document.getElementById('student-name').value;
        const teacherEmail = document.getElementById('teacher-email').value;

        const subject = encodeURIComponent(`Unit 7 Quiz Results: ${name}`);
        const body = encodeURIComponent(`Student Name: ${name}\nFinal Score: ${score} / 17`);

        // Lock the quiz
        localStorage.setItem(STORAGE_KEY, score);
        
        // Open Mail Client
        window.location.href = `mailto:${teacherEmail}?subject=${subject}&body=${body}`;
        
        showFinish(score);
    }
</script>
</body>
</html>
