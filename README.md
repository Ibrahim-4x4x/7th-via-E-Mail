<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Unit 7: Communication Interactive Activities</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body { background-color: #f0f4f8; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; }
        .quiz-card { background: white; border-radius: 1.5rem; box-shadow: 0 10px 25px rgba(0,0,0,0.1); }
        .question-block { border-bottom: 1px solid #edf2f7; padding-bottom: 1.5rem; margin-bottom: 1.5rem; }
    </style>
</head>
<body class="p-4 md:p-8">

<div class="max-w-4xl mx-auto quiz-card p-6 md:p-10">
    <div id="start-screen" class="text-center py-10">
        <div class="mb-6 inline-block p-4 bg-blue-100 rounded-full">
            <svg class="w-12 h-12 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 12h.01M12 12h.01M16 12h.01M21 12c0 4.418-4.03 8-9 8a9.863 9.863 0 01-4.255-.949L3 20l1.395-3.72C3.512 15.042 3 13.574 3 12c0-4.418 4.03-8 9-8s9 3.582 9 8z"></path></svg>
        </div>
        <h1 class="text-4xl font-bold text-blue-900 mb-2">Unit 7: Let's Talk!</h1>
        <p class="text-gray-600 mb-8 text-lg">Complete all exercises from Lessons 1 & 2</p>
        
        <div class="space-y-4 max-w-md mx-auto bg-gray-50 p-6 rounded-2xl border border-gray-200">
            <input type="text" id="student-name" class="w-full p-3 border rounded-lg outline-none focus:ring-2 focus:ring-blue-400" placeholder="Student Full Name">
            <input type="email" id="teacher-email" class="w-full p-3 border rounded-lg outline-none focus:ring-2 focus:ring-red-400" placeholder="Teacher's Email Address">
            <button onclick="initQuiz()" class="w-full bg-blue-600 text-white py-4 rounded-xl font-bold hover:bg-blue-700 transition transform hover:scale-105 shadow-lg">Start All Activities</button>
        </div>
    </div>

    <div id="quiz-screen" class="hidden">
        <div class="flex justify-between items-center mb-8 sticky top-0 bg-white/90 backdrop-blur-sm py-4 border-b z-10">
            <div>
                <span class="font-bold text-blue-700 block" id="display-name"></span>
                <span class="text-xs text-gray-500 uppercase tracking-widest">Unit 7 Communication</span>
            </div>
            <div class="text-right">
                <span class="bg-blue-600 text-white px-4 py-2 rounded-full text-sm font-bold">Total Items: 40</span>
            </div>
        </div>

        <form id="quiz-form">
            <div class="mb-12">
                <h2 class="text-2xl font-black text-blue-800 mb-6 flex items-center">
                    <span class="bg-blue-800 text-white w-8 h-8 rounded-md flex items-center justify-center mr-3 text-sm">1</span>
                    Lesson 1: Vocabulary
                </h2>
                
                <div class="grid md:grid-cols-2 gap-6">
                    <div class="p-4 bg-gray-50 rounded-xl">
                        <p class="font-medium mb-3">1. I'm going to ______ to a podcast.</p>
                        <select name="l1_q1" class="w-full p-2 border rounded">
                            <option value="">Select...</option>
                            <option value="insert">insert</option>
                            <option value="listen">listen</option>
                            <option value="use">use</option>
                        </select>
                    </div>
                    <div class="p-4 bg-gray-50 rounded-xl">
                        <p class="font-medium mb-3">2. Lisa likes to ______ to friends online.</p>
                        <select name="l1_q2" class="w-full p-2 border rounded">
                            <option value="">Select...</option>
                            <option value="chat">chat</option>
                            <option value="receive">receive</option>
                            <option value="get">get</option>
                        </select>
                    </div>
                    <div class="p-4 bg-gray-50 rounded-xl">
                        <p class="font-medium mb-3">3. Dad doesn't like ______ social media.</p>
                        <select name="l1_q3" class="w-full p-2 border rounded">
                            <option value="">Select...</option>
                            <option value="writing">writing</option>
                            <option value="using">using</option>
                            <option value="seeing">seeing</option>
                        </select>
                    </div>
                    <div class="p-4 bg-gray-50 rounded-xl">
                        <p class="font-medium mb-3">4. We'd like to ______ a vlog about UAE.</p>
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
                <h2 class="text-2xl font-black text-blue-800 mb-6 flex items-center">
                    <span class="bg-blue-800 text-white w-8 h-8 rounded-md flex items-center justify-center mr-3 text-sm">2</span>
                    Unscramble Survey Questions
                </h2>
                <div class="space-y-4">
                    <div class="flex items-center space-x-4 p-3 bg-white border rounded-lg">
                        <span class="text-gray-400 font-bold">Q2</span>
                        <p class="flex-1">Do you often <span class="text-blue-600 font-mono">[ceevrie xett samsegse]</span></p>
                        <input type="text" name="l1_u1" class="border-b-2 border-blue-200 outline-none focus:border-blue-500 p-1" placeholder="Type here...">
                    </div>
                    <div class="flex items-center space-x-4 p-3 bg-white border rounded-lg">
                        <span class="text-gray-400 font-bold">Q3</span>
                        <p class="flex-1">Could you <span class="text-blue-600 font-mono">[pkee a creste]</span> if told one?</p>
                        <input type="text" name="l1_u2" class="border-b-2 border-blue-200 outline-none focus:border-blue-500 p-1" placeholder="Type here...">
                    </div>
                    <div class="flex items-center space-x-4 p-3 bg-white border rounded-lg">
                        <span class="text-gray-400 font-bold">Q4</span>
                        <p class="flex-1">Do you usually <span class="text-blue-600 font-mono">[itle eth utthr]</span> to friends?</p>
                        <input type="text" name="l1_u3" class="border-b-2 border-blue-200 outline-none focus:border-blue-500 p-1" placeholder="Type here...">
                    </div>
                </div>
            </div>

            <div class="mb-12">
                <h2 class="text-2xl font-black text-blue-800 mb-6 flex items-center">
                    <span class="bg-blue-800 text-white w-8 h-8 rounded-md flex items-center justify-center mr-3 text-sm">3</span>
                    Opposites
                </h2>
                <div class="bg-indigo-50 p-6 rounded-2xl border border-indigo-100 space-y-4">
                    <p>1. If you can't keep a secret, people won't <input type="text" name="opp_1" class="w-20 border-b border-indigo-400 bg-transparent text-center" placeholder="???"> you any.</p>
                    <p>2. I don't get on well with him. We usually get on <input type="text" name="opp_2" class="w-20 border-b border-indigo-400 bg-transparent text-center" placeholder="???">.</p>
                    <p>3. I can't receive or <input type="text" name="opp_3" class="w-20 border-b border-indigo-400 bg-transparent text-center" placeholder="???"> a text message.</p>
                    <p>4. You shouldn't tell lies, you should always tell the <input type="text" name="opp_4" class="w-20 border-b border-indigo-400 bg-transparent text-center" placeholder="???">.</p>
                    <p>5. You should try to <input type="text" name="opp_5" class="w-20 border-b border-indigo-400 bg-transparent text-center" placeholder="???"> a promise. Don't break it.</p>
                </div>
            </div>

            <div class="mb-12">
                <h2 class="text-2xl font-black text-blue-800 mb-6 flex items-center">
                    <span class="bg-blue-800 text-white w-8 h-8 rounded-md flex items-center justify-center mr-3 text-sm">4</span>
                    Lesson 2: Dialogue Completion
                </h2>
                <div class="grid grid-cols-2 md:grid-cols-4 gap-2 mb-6">
                    <span class="bg-gray-200 text-xs p-1 rounded text-center">angry</span> <span class="bg-gray-200 text-xs p-1 rounded text-center">arguments</span>
                    <span class="bg-gray-200 text-xs p-1 rounded text-center">borrow</span> <span class="bg-gray-200 text-xs p-1 rounded text-center">cool</span>
                    <span class="bg-gray-200 text-xs p-1 rounded text-center">easy</span> <span class="bg-gray-200 text-xs p-1 rounded text-center">experiences</span>
                    <span class="bg-gray-200 text-xs p-1 rounded text-center">huge</span> <span class="bg-gray-200 text-xs p-1 rounded text-center">maybe</span>
                    <span class="bg-gray-200 text-xs p-1 rounded text-center">month</span> <span class="bg-gray-200 text-xs p-1 rounded text-center">podcasts</span>
                    <span class="bg-gray-200 text-xs p-1 rounded text-center">trying</span> <span class="bg-gray-200 text-xs p-1 rounded text-center">vlogs</span>
                </div>
                <div class="space-y-4 text-gray-700 italic">
                    <p>1. I'm <input type="text" name="d1" class="border-b border-gray-400 w-24 text-center not-italic"> to get on well with everyone for a <input type="text" name="d2" class="border-b border-gray-400 w-24 text-center not-italic">.</p>
                    <p>2. Well, it's been <input type="text" name="d3" class="border-b border-gray-400 w-24 text-center not-italic"> with my friends. I haven't had any <input type="text" name="d4" class="border-b border-gray-400 w-24 text-center not-italic"> with them.</p>
                    <p>3. I was so <input type="text" name="d5" class="border-b border-gray-400 w-24 text-center not-italic"> and we had a <input type="text" name="d6" class="border-b border-gray-400 w-24 text-center not-italic"> argument!</p>
                    <p>4. <input type="text" name="d7" class="border-b border-gray-400 w-24 text-center not-italic"> you should record your <input type="text" name="d8" class="border-b border-gray-400 w-24 text-center not-italic"> in some way.</p>
                    <p>5. I think <input type="text" name="d9" class="border-b border-gray-400 w-24 text-center not-italic"> will be as popular as <input type="text" name="d10" class="border-b border-gray-400 w-24 text-center not-italic"> one day.</p>
                    <p>6. I think it's a <input type="text" name="d11" class="border-b border-gray-400 w-24 text-center not-italic"> T-shirt! Just don't let my sister <input type="text" name="d12" class="border-b border-gray-400 w-24 text-center not-italic"> it!</p>
                </div>
            </div>

            <div class="mb-12">
                <h2 class="text-2xl font-black text-blue-800 mb-6 flex items-center">
                    <span class="bg-blue-800 text-white w-8 h-8 rounded-md flex items-center justify-center mr-3 text-sm">5</span>
                    True or False?
                </h2>
                <div class="space-y-4">
                    <div class="flex justify-between items-center p-3 bg-gray-50 rounded-lg">
                        <span>1. Dana has been doing an experiment for a week.</span>
                        <div class="space-x-4">
                            <label><input type="radio" name="tf1" value="T"> T</label>
                            <label><input type="radio" name="tf1" value="F"> F</label>
                        </div>
                    </div>
                    <div class="flex justify-between items-center p-3 bg-gray-50 rounded-lg">
                        <span>2. Dana gets on worse with her sister than friends.</span>
                        <div class="space-x-4">
                            <label><input type="radio" name="tf2" value="T"> T</label>
                            <label><input type="radio" name="tf2" value="F"> F</label>
                        </div>
                    </div>
                </div>
            </div>

            <button type="button" onclick="submitToEmail()" class="w-full bg-red-600 text-white py-5 rounded-2xl font-bold text-2xl hover:bg-red-700 transition shadow-xl transform hover:-translate-y-1">Submit All Results</button>
        </form>
    </div>

    <div id="finish-screen" class="hidden text-center py-20">
        <div class="text-8xl mb-6">🎉</div>
        <h2 class="text-4xl font-bold text-gray-800 mb-4">Well Done!</h2>
        <p id="score-display" class="text-5xl text-blue-600 font-black mb-6"></p>
        <p class="text-gray-500 mb-8">Your work has been graded and prepared for your teacher.</p>
        <button onclick="location.reload()" class="bg-gray-200 px-6 py-2 rounded-full text-gray-600 hover:bg-gray-300">Restart Activity</button>
    </div>
</div>

<script>
    const STORAGE_KEY = 'unit7_full_quiz_lock';

    function initQuiz() {
        const name = document.getElementById('student-name').value;
        const email = document.getElementById('teacher-email').value;
        if (!name.trim() || !email.trim()) { alert("Please enter your name and teacher's email!"); return; }
        
        document.getElementById('start-screen').classList.add('hidden');
        document.getElementById('quiz-screen').classList.remove('hidden');
        document.getElementById('display-name').innerText = "Student: " + name;
        window.scrollTo(0,0);
    }

    function calculateScore() {
        const form = document.getElementById('quiz-form');
        const data = new FormData(form);
        let score = 0;

        // Lesson 1 Logic
        if (data.get('l1_q1') === 'listen') score++;
        if (data.get('l1_q2') === 'chat') score++;
        if (data.get('l1_q3') === 'using') score++;
        if (data.get('l1_q4') === 'watch') score++;
        
        // Unscramble Logic (Trim and Lowercase)
        if (data.get('l1_u1')?.toLowerCase().trim() === 'receive text messages') score++;
        if (data.get('l1_u2')?.toLowerCase().trim() === 'keep a secret') score++;
        if (data.get('l1_u3')?.toLowerCase().trim() === 'tell the truth') score++;

        // Opposites Logic
        if (data.get('opp_1')?.toLowerCase().trim() === 'tell') score++;
        if (data.get('opp_2')?.toLowerCase().trim() === 'on badly' || data.get('opp_2')?.toLowerCase().trim() === 'badly') score++;
        if (data.get('opp_3')?.toLowerCase().trim() === 'send') score++;
        if (data.get('opp_4')?.toLowerCase().trim() === 'truth') score++;
        if (data.get('opp_5')?.toLowerCase().trim() === 'keep') score++;

        // Dialogue Logic
        const dialogueAnswers = ['trying','month','easy','arguments','angry','huge','maybe','experiences','podcasts','vlogs','cool','borrow'];
        for(let i=1; i<=12; i++) {
            if (data.get('d'+i)?.toLowerCase().trim() === dialogueAnswers[i-1]) score++;
        }

        // T/F Logic
        if (data.get('tf1') === 'F') score++;
        if (data.get('tf2') === 'T') score++;

        return score;
    }

    function submitToEmail() {
        const score = calculateScore();
        const total = 26; // Adjusted based on questions included
        const name = document.getElementById('student-name').value;
        const teacherEmail = document.getElementById('teacher-email').value;

        const subject = encodeURIComponent(`Unit 7 Communication Results - ${name}`);
        const body = encodeURIComponent(`Student: ${name}\nScore: ${score} / ${total}\n\nCompleted exercises for Lesson 1 and Lesson 2.`);

        window.location.href = `mailto:${teacherEmail}?subject=${subject}&body=${body}`;
        
        document.getElementById('quiz-screen').classList.add('hidden');
        document.getElementById('finish-screen').classList.remove('hidden');
        document.getElementById('score-display').innerText = `${score} / ${total}`;
    }
</script>
</body>
</html>
