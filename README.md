<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Unit 7 Interactive Workbook</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body { background-color: #f3f4f6; font-family: 'Inter', sans-serif; }
        .quiz-card { background: white; border-radius: 1.5rem; box-shadow: 0 10px 25px rgba(0,0,0,0.1); }
        .input-focus { outline: none; border-bottom: 2px solid #3b82f6; background: transparent; }
        .hidden { display: none; }
    </style>
</head>
<body class="p-4 md:p-10">

<div class="max-w-4xl mx-auto quiz-card p-6 md:p-12">
    <div id="start-screen" class="text-center py-10">
        <h1 class="text-4xl font-extrabold text-blue-900 mb-4">Unit 7: Let's Talk!</h1>
        <p class="text-gray-500 mb-8 text-lg">Complete all exercises from Lessons 1 & 2</p>
        
        <div class="space-y-4 max-w-sm mx-auto">
            <input type="text" id="student-name" class="w-full p-4 border rounded-xl outline-none focus:ring-2 focus:ring-blue-400" placeholder="Your Full Name">
            <input type="email" id="teacher-email" class="w-full p-4 border rounded-xl outline-none focus:ring-2 focus:ring-red-400" placeholder="Teacher's Email">
            <button onclick="initQuiz()" class="w-full bg-blue-600 text-white py-4 rounded-xl font-bold hover:bg-blue-700 transition transform hover:scale-105 shadow-lg">
                Begin Activities
            </button>
        </div>
        <p class="text-xs text-red-500 mt-6 font-medium">⚠️ Important: You can only submit your answers once.</p>
    </div>

    <div id="quiz-screen" class="hidden">
        <header class="flex justify-between items-center mb-10 border-b pb-4 sticky top-0 bg-white/90 backdrop-blur-sm z-20">
            <div>
                <p class="text-blue-600 font-bold uppercase tracking-widest text-xs">Student Portal</p>
                <h2 id="display-name" class="text-xl font-black text-gray-800"></h2>
            </div>
            <div class="text-right">
                <span class="bg-gray-100 px-3 py-1 rounded-md text-sm font-bold text-gray-600">Unit 7: Communication</span>
            </div>
        </header>

        <form id="quiz-form">
            <section class="mb-12">
                <h3 class="text-xl font-bold text-blue-800 mb-4 flex items-center">
                    <span class="bg-blue-100 text-blue-600 w-8 h-8 rounded-full flex items-center justify-center mr-3">1</span>
                    Vocabulary: Circle the correct options
                </h3>
                <div class="grid gap-4 md:grid-cols-2">
                    <div class="p-4 bg-blue-50 rounded-lg">
                        <p>1. I'm going to <select name="v1" class="rounded border p-1 mx-1"><option value="">...</option><option value="insert">insert</option><option value="listen">listen</option><option value="use">use</option></select> to a podcast.</p>
                    </div>
                    <div class="p-4 bg-blue-50 rounded-lg">
                        <p>2. Lisa likes to <select name="v2" class="rounded border p-1 mx-1"><option value="">...</option><option value="chat">chat</option><option value="receive">receive</option><option value="get">get</option></select> to friends online.</p>
                    </div>
                    <div class="p-4 bg-blue-50 rounded-lg">
                        <p>3. Dad doesn't like <select name="v3" class="rounded border p-1 mx-1"><option value="">...</option><option value="writing">writing</option><option value="using">using</option><option value="seeing">seeing</option></select> social media.</p>
                    </div>
                    <div class="p-4 bg-blue-50 rounded-lg">
                        <p>4. We'd like to <select name="v4" class="rounded border p-1 mx-1"><option value="">...</option><option value="watch">watch</option><option value="get">get</option><option value="use">use</option></select> a vlog about UAE.</p>
                    </div>
                </div>
            </section>

            <section class="mb-12">
                <h3 class="text-xl font-bold text-blue-800 mb-4 flex items-center">
                    <span class="bg-blue-100 text-blue-600 w-8 h-8 rounded-full flex items-center justify-center mr-3">2</span>
                    Unscramble the Survey Questions
                </h3>
                <div class="space-y-4">
                    <div class="flex items-center gap-2 p-3 border-b">
                        <span class="font-bold text-gray-400">Q1:</span>
                        <p class="flex-grow">Do you often <input type="text" name="u1" placeholder="[ceevrie xett samsegse]" class="input-focus w-full max-w-md ml-2"></p>
                    </div>
                    <div class="flex items-center gap-2 p-3 border-b">
                        <span class="font-bold text-gray-400">Q2:</span>
                        <p class="flex-grow">Could you <input type="text" name="u2" placeholder="[pkee a creste]" class="input-focus w-full max-w-md ml-2"> if told one?</p>
                    </div>
                    <div class="flex items-center gap-2 p-3 border-b">
                        <span class="font-bold text-gray-400">Q3:</span>
                        <p class="flex-grow">Do you usually <input type="text" name="u3" placeholder="[itle eth utthr]" class="input-focus w-full max-w-md ml-2"> to friends?</p>
                    </div>
                </div>
            </section>

            <section class="mb-12">
                <h3 class="text-xl font-bold text-blue-800 mb-4">Opposites (badly, keep, truth, send, tell)</h3>
                <div class="bg-gray-50 p-6 rounded-2xl space-y-4">
                    <p>1. If you can't keep a secret, people won't <input type="text" name="op1" class="border-b border-gray-400 w-24 text-center"> you any.</p>
                    <p>2. I don't get on well with Hassan. We usually get on <input type="text" name="op2" class="border-b border-gray-400 w-24 text-center">.</p>
                    <p>3. I can't receive or <input type="text" name="op3" class="border-b border-gray-400 w-24 text-center"> a text message.</p>
                    <p>4. You shouldn't tell lies, you should always tell the <input type="text" name="op4" class="border-b border-gray-400 w-24 text-center">.</p>
                </div>
            </section>

            <section class="mb-12">
                <h3 class="text-xl font-bold text-blue-800 mb-4 flex items-center">
                    <span class="bg-blue-100 text-blue-600 w-8 h-8 rounded-full flex items-center justify-center mr-3">3</span>
                    Lesson 2: Dialogue Completion
                </h3>
                <div class="bg-indigo-900 text-white p-4 rounded-xl text-xs mb-4 flex flex-wrap gap-2">
                    <span>angry</span> <span>arguments</span> <span>borrow</span> <span>cool</span> <span>easy</span> <span>experiences</span>
                    <span>huge</span> <span>maybe</span> <span>month</span> <span>podcasts</span> <span>trying</span> <span>vlogs</span>
                </div>
                <div class="space-y-4 italic text-gray-700">
                    <p>1. I'm <input type="text" name="d1" class="border-b border-blue-300 w-24 text-center"> to get on well with everyone for a <input type="text" name="d2" class="border-b border-blue-300 w-24 text-center">.</p>
                    <p>2. Well, it's been <input type="text" name="d3" class="border-b border-blue-300 w-24 text-center"> with my friends. I haven't had any <input type="text" name="d4" class="border-b border-blue-300 w-24 text-center"> with them.</p>
                    <p>3. I was so <input type="text" name="d5" class="border-b border-blue-300 w-24 text-center"> and we had a <input type="text" name="d6" class="border-b border-blue-300 w-24 text-center"> argument!</p>
                    <p>4. <input type="text" name="d7" class="border-b border-blue-300 w-24 text-center"> you should record your <input type="text" name="d8" class="border-b border-blue-300 w-24 text-center"> in some way.</p>
                    <p>5. I think <input type="text" name="d9" class="border-b border-blue-300 w-24 text-center"> will be as popular as <input type="text" name="d10" class="border-b border-blue-300 w-24 text-center"> one day.</p>
                </div>
            </section>

            <section class="mb-12">
                <h3 class="text-xl font-bold text-blue-800 mb-4">True or False</h3>
                <div class="space-y-3">
                    <div class="flex justify-between p-3 bg-gray-50 rounded">
                        <span>1. Dana has been doing an experiment for a week.</span>
                        <div>
                            <label class="mr-2"><input type="radio" name="tf1" value="T"> T</label>
                            <label><input type="radio" name="tf1" value="F"> F</label>
                        </div>
                    </div>
                    <div class="flex justify-between p-3 bg-gray-50 rounded">
                        <span>2. Dana gets on worse with her sister than friends.</span>
                        <div>
                            <label class="mr-2"><input type="radio" name="tf2" value="T"> T</label>
                            <label><input type="radio" name="tf2" value="F"> F</label>
                        </div>
                    </div>
                </div>
            </section>

            <button type="button" onclick="submitToEmail()" class="w-full bg-green-600 text-white py-5 rounded-2xl font-black text-2xl hover:bg-green-700 transition shadow-xl transform hover:-translate-y-1">
                SUBMIT WORK
            </button>
        </form>
    </div>

    <div id="finish-screen" class="hidden text-center py-20">
        <div class="text-8xl mb-6">🎯</div>
        <h2 class="text-4xl font-bold text-gray-800 mb-2">Workbook Submitted!</h2>
        <p id="score-display" class="text-5xl text-blue-600 font-black mb-6"></p>
        <div class="bg-blue-50 p-6 rounded-xl max-w-md mx-auto border border-blue-100">
            <p class="text-blue-800">Your answers are now locked. Your teacher has been notified of your completion.</p>
        </div>
    </div>
</div>

<script>
    const LOCK_KEY = 'unit7_workbook_locked';

    window.onload = () => {
        const savedScore = localStorage.getItem(LOCK_KEY);
        if (savedScore) {
            showFinish(savedScore);
        }
    };

    function initQuiz() {
        const name = document.getElementById('student-name').value;
        const email = document.getElementById('teacher-email').value;
        if (!name.trim() || !email.trim()) { alert("Please enter both Name and Email!"); return; }
        
        document.getElementById('start-screen').classList.add('hidden');
        document.getElementById('quiz-screen').classList.remove('hidden');
        document.getElementById('display-name').innerText = name;
        window.scrollTo(0,0);
    }

    function calculateScore() {
        const data = new FormData(document.getElementById('quiz-form'));
        let score = 0;

        // Scoring Logic
        if (data.get('v1') === 'listen') score++;
        if (data.get('v2') === 'chat') score++;
        if (data.get('v3') === 'using') score++;
        if (data.get('v4') === 'watch') score++;
        
        if (data.get('u1')?.toLowerCase().includes('receive text messages')) score++;
        if (data.get('u2')?.toLowerCase().includes('keep a secret')) score++;
        if (data.get('u3')?.toLowerCase().includes('tell the truth')) score++;

        if (data.get('op1')?.toLowerCase() === 'tell') score++;
        if (data.get('op2')?.toLowerCase() === 'badly') score++;
        if (data.get('op3')?.toLowerCase() === 'send') score++;
        if (data.get('op4')?.toLowerCase() === 'truth') score++;

        const dialogue = ['trying','month','easy','arguments','angry','huge','maybe','experiences','podcasts','vlogs'];
        for(let i=1; i<=10; i++) {
            if (data.get('d'+i)?.toLowerCase().trim() === dialogue[i-1]) score++;
        }

        if (data.get('tf1') === 'F') score++;
        if (data.get('tf2') === 'T') score++;

        return score;
    }

    function submitToEmail() {
        const score = calculateScore();
        const total = 23;
        const name = document.getElementById('student-name').value;
        const teacherEmail = document.getElementById('teacher-email').value;

        // Save Lock
        localStorage.setItem(LOCK_KEY, `${score}/${total}`);

        // Trigger Email
        const subject = encodeURIComponent(`Unit 7 Workbook: ${name}`);
        const body = encodeURIComponent(`Student: ${name}\nScore: ${score} / ${total}\n\nThis student has completed Lesson 1 and 2 activities.`);
        window.location.href = `mailto:${teacherEmail}?subject=${subject}&body=${body}`;

        showFinish(`${score}/${total}`);
    }

    function showFinish(scoreText) {
        document.getElementById('start-screen').classList.add('hidden');
        document.getElementById('quiz-screen').classList.add('hidden');
        document.getElementById('finish-screen').classList.remove('hidden');
        document.getElementById('score-display').innerText = scoreText;
    }
</script>
</body>
</html>
