<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Edavankattil Family Heritage</title>
    <link href="https://fonts.googleapis.com/css2?family=Crimson+Pro:wght@300;400;600;700&family=Cormorant+Garamond:wght@400;600;700&family=Montserrat:wght@400;500;600&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary-bg: #faf8f3;
            --secondary-bg: #f5f1e8;
            --accent-gold: #d4a574;
            --accent-bronze: #b8956a;
            --text-dark: #2c2416;
            --text-light: #5a4f3d;
            --gen-1: linear-gradient(135deg, #8b4513 0%, #a0522d 100%);
            --gen-2: linear-gradient(135deg, #2c5f7a 0%, #4a7c9e 100%);
            --gen-3: linear-gradient(135deg, #3e6b47 0%, #5a8f62 100%);
            --gen-4: linear-gradient(135deg, #8b6f47 0%, #a68a5e 100%);
            --gen-5: linear-gradient(135deg, #6b7280 0%, #8b95a1 100%);
        }

        body {
            font-family: 'Crimson Pro', serif;
            background: var(--primary-bg);
            background-image: 
                radial-gradient(circle at 20% 50%, rgba(212, 165, 116, 0.05) 0%, transparent 50%),
                radial-gradient(circle at 80% 80%, rgba(184, 149, 106, 0.05) 0%, transparent 50%);
            min-height: 100vh;
            color: var(--text-dark);
            line-height: 1.6;
        }

        .heritage-container {
            max-width: 1600px;
            margin: 0 auto;
            padding: 20px;
        }

        /* Header Section */
        .heritage-header {
            text-align: center;
            padding: 60px 40px;
            background: linear-gradient(135deg, rgba(44, 36, 22, 0.95) 0%, rgba(90, 79, 61, 0.9) 100%);
            border-radius: 30px;
            margin-bottom: 40px;
            position: relative;
            overflow: hidden;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.15);
        }

        .heritage-header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg width="100" height="100" xmlns="http://www.w3.org/2000/svg"><defs><pattern id="grid" width="50" height="50" patternUnits="userSpaceOnUse"><path d="M 50 0 L 0 0 0 50" fill="none" stroke="rgba(212,165,116,0.1)" stroke-width="1"/></pattern></defs><rect width="100" height="100" fill="url(%23grid)"/></svg>');
            opacity: 0.3;
        }

        .heritage-header h1 {
            font-family: 'Cormorant Garamond', serif;
            font-size: 4em;
            font-weight: 700;
            color: var(--accent-gold);
            margin-bottom: 15px;
            position: relative;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
            letter-spacing: 2px;
        }

        .heritage-subtitle {
            font-size: 1.4em;
            color: rgba(255, 255, 255, 0.9);
            font-weight: 300;
            position: relative;
            letter-spacing: 3px;
            text-transform: uppercase;
            font-family: 'Montserrat', sans-serif;
            font-size: 0.9em;
        }

        .heritage-ornament {
            width: 100px;
            height: 3px;
            background: var(--accent-gold);
            margin: 25px auto;
            position: relative;
        }

        .heritage-ornament::before,
        .heritage-ornament::after {
            content: '◆';
            position: absolute;
            color: var(--accent-gold);
            font-size: 12px;
            top: -8px;
        }

        .heritage-ornament::before {
            left: -20px;
        }

        .heritage-ornament::after {
            right: -20px;
        }

        /* Controls Panel */
        .controls-panel {
            background: white;
            border-radius: 25px;
            padding: 35px;
            margin-bottom: 40px;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.08);
            border: 1px solid rgba(212, 165, 116, 0.2);
        }

        .search-container {
            display: flex;
            gap: 15px;
            margin-bottom: 25px;
            flex-wrap: wrap;
        }

        .search-input {
            flex: 1;
            min-width: 250px;
            padding: 16px 24px;
            border: 2px solid var(--secondary-bg);
            border-radius: 50px;
            font-size: 16px;
            font-family: 'Crimson Pro', serif;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            background: var(--secondary-bg);
        }

        .search-input:focus {
            outline: none;
            border-color: var(--accent-gold);
            background: white;
            box-shadow: 0 5px 20px rgba(212, 165, 116, 0.15);
        }

        .heritage-btn {
            padding: 16px 32px;
            border: none;
            border-radius: 50px;
            font-family: 'Montserrat', sans-serif;
            font-size: 14px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .btn-primary {
            background: linear-gradient(135deg, var(--accent-gold) 0%, var(--accent-bronze) 100%);
            color: white;
            box-shadow: 0 4px 15px rgba(212, 165, 116, 0.3);
        }

        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 25px rgba(212, 165, 116, 0.4);
        }

        .btn-secondary {
            background: var(--secondary-bg);
            color: var(--text-dark);
        }

        .btn-secondary:hover {
            background: #e8e4d8;
            transform: translateY(-2px);
        }

        .button-group {
            display: flex;
            gap: 12px;
            justify-content: center;
            flex-wrap: wrap;
        }

        /* Legend */
        .generation-legend {
            display: flex;
            gap: 25px;
            justify-content: center;
            flex-wrap: wrap;
            margin-top: 25px;
            padding-top: 25px;
            border-top: 2px solid var(--secondary-bg);
        }

        .legend-badge {
            display: flex;
            align-items: center;
            gap: 12px;
            padding: 12px 20px;
            background: var(--secondary-bg);
            border-radius: 50px;
            font-size: 14px;
            font-family: 'Montserrat', sans-serif;
            font-weight: 500;
            transition: transform 0.3s;
        }

        .legend-badge:hover {
            transform: scale(1.05);
        }

        .legend-color-box {
            width: 35px;
            height: 35px;
            border-radius: 10px;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.15);
        }

        .gen-1-color { background: var(--gen-1); }
        .gen-2-color { background: var(--gen-2); }
        .gen-3-color { background: var(--gen-3); }
        .gen-4-color { background: var(--gen-4); }
        .gen-5-color { background: var(--gen-5); }

        /* Tree Structure */
        .tree-container {
            padding: 40px 20px;
        }

        .tree-list {
            list-style: none;
        }

        .tree-node {
            margin: 20px 0;
        }

        /* Member Card */
        .member-card {
            background: white;
            border-radius: 20px;
            padding: 20px 28px;
            box-shadow: 0 8px 30px rgba(0, 0, 0, 0.08);
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            cursor: pointer;
            display: inline-flex;
            align-items: center;
            gap: 20px;
            margin: 8px 0;
            position: relative;
            border: 2px solid transparent;
            max-width: 600px;
        }

        .member-card:hover {
            transform: translateX(8px) translateY(-4px);
            box-shadow: 0 15px 50px rgba(0, 0, 0, 0.12);
        }

        .member-card.highlighted {
            border-color: var(--accent-gold);
            background: linear-gradient(135deg, #fff9f0 0%, white 100%);
            animation: highlight-pulse 1.5s ease-in-out 3;
        }

        @keyframes highlight-pulse {
            0%, 100% { transform: scale(1); box-shadow: 0 8px 30px rgba(212, 165, 116, 0.2); }
            50% { transform: scale(1.02); box-shadow: 0 12px 40px rgba(212, 165, 116, 0.35); }
        }

        .member-avatar {
            width: 60px;
            height: 60px;
            border-radius: 15px;
            flex-shrink: 0;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-weight: 700;
            font-size: 24px;
            font-family: 'Cormorant Garamond', serif;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.15);
            position: relative;
        }

        .gen-1-card .member-avatar { background: var(--gen-1); }
        .gen-2-card .member-avatar { background: var(--gen-2); }
        .gen-3-card .member-avatar { background: var(--gen-3); }
        .gen-4-card .member-avatar { background: var(--gen-4); }
        .gen-5-card .member-avatar { background: var(--gen-5); }

        .member-info {
            flex: 1;
            min-width: 0;
        }

        .member-name {
            font-size: 1.3em;
            font-weight: 600;
            color: var(--text-dark);
            margin-bottom: 4px;
            font-family: 'Cormorant Garamond', serif;
        }

        .member-spouse {
            color: var(--text-light);
            font-size: 0.95em;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .marriage-icon {
            color: var(--accent-gold);
            font-weight: bold;
        }

        .expand-indicator {
            width: 35px;
            height: 35px;
            border-radius: 10px;
            background: var(--secondary-bg);
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 700;
            color: var(--text-dark);
            transition: all 0.3s;
            font-size: 18px;
        }

        .member-card:hover .expand-indicator {
            background: var(--accent-gold);
            color: white;
            transform: scale(1.1);
        }

        /* Branch Coordinator Badge */
        .coordinator-badge {
            background: linear-gradient(135deg, #fff9f0 0%, #fff5e6 100%);
            border-left: 4px solid var(--accent-gold);
            padding: 15px 20px;
            border-radius: 12px;
            margin: 15px 0;
            display: inline-flex;
            align-items: center;
            gap: 12px;
            font-family: 'Montserrat', sans-serif;
            font-size: 14px;
            color: var(--text-dark);
            box-shadow: 0 3px 15px rgba(212, 165, 116, 0.1);
        }

        .coordinator-icon {
            font-size: 20px;
        }

        /* Children Container */
        .children-container {
            list-style: none;
            margin-left: 50px;
            padding-left: 30px;
            border-left: 3px solid rgba(212, 165, 116, 0.2);
            position: relative;
            display: none;
        }

        .children-container::before {
            content: '';
            position: absolute;
            left: -3px;
            top: 0;
            width: 3px;
            height: 30px;
            background: linear-gradient(180deg, var(--accent-gold) 0%, transparent 100%);
        }

        .children-container.expanded {
            display: block;
            animation: slideDown 0.5s cubic-bezier(0.4, 0, 0.2, 1);
        }

        @keyframes slideDown {
            from {
                opacity: 0;
                transform: translateY(-20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Simple children list */
        .children-list {
            background: linear-gradient(135deg, #fafaf8 0%, white 100%);
            padding: 20px 25px;
            border-radius: 15px;
            margin: 12px 0;
            border: 1px solid rgba(212, 165, 116, 0.15);
            font-size: 0.95em;
            line-height: 1.8;
        }

        .children-list::before {
            content: '→';
            color: var(--accent-gold);
            font-weight: bold;
            margin-right: 10px;
            font-size: 1.2em;
        }

        /* Generation Badge */
        .gen-badge {
            position: absolute;
            top: 10px;
            right: 15px;
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 11px;
            font-weight: 600;
            font-family: 'Montserrat', sans-serif;
            text-transform: uppercase;
            letter-spacing: 0.5px;
            background: var(--secondary-bg);
            color: var(--text-light);
        }

        /* Responsive */
        @media (max-width: 768px) {
            .heritage-header h1 {
                font-size: 2.5em;
            }
            
            .heritage-header {
                padding: 40px 20px;
            }
            
            .controls-panel {
                padding: 25px 20px;
            }
            
            .member-card {
                max-width: 100%;
                padding: 18px 20px;
            }
            
            .member-avatar {
                width: 50px;
                height: 50px;
                font-size: 20px;
            }
            
            .member-name {
                font-size: 1.1em;
            }
            
            .children-container {
                margin-left: 25px;
                padding-left: 20px;
            }
            
            .generation-legend {
                gap: 15px;
            }
            
            .legend-badge {
                padding: 10px 16px;
                font-size: 12px;
            }
        }

        /* Scroll effects */
        .fade-in {
            animation: fadeIn 0.6s ease-out;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
</head>
<body>
    <div class="heritage-container">
        <!-- Header -->
        <div class="heritage-header fade-in">
            <h1>Edavankattil</h1>
            <div class="heritage-ornament"></div>
            <p class="heritage-subtitle">Family Heritage Archive</p>
        </div>

        <!-- Controls -->
        <div class="controls-panel fade-in">
            <div class="search-container">
                <input 
                    type="text" 
                    class="search-input" 
                    id="searchInput" 
                    placeholder="Search for family members..."
                >
                <button class="heritage-btn btn-primary" onclick="searchFamily()">Search</button>
                <button class="heritage-btn btn-secondary" onclick="clearSearch()">Clear</button>
            </div>
            
            <div class="button-group">
                <button class="heritage-btn btn-secondary" onclick="expandAll()">Expand All Branches</button>
                <button class="heritage-btn btn-secondary" onclick="collapseAll()">Collapse All</button>
            </div>

            <div class="generation-legend">
                <div class="legend-badge">
                    <div class="legend-color-box gen-1-color"></div>
                    <span>Generation 1</span>
                </div>
                <div class="legend-badge">
                    <div class="legend-color-box gen-2-color"></div>
                    <span>Generation 2</span>
                </div>
                <div class="legend-badge">
                    <div class="legend-color-box gen-3-color"></div>
                    <span>Generation 3</span>
                </div>
                <div class="legend-badge">
                    <div class="legend-color-box gen-4-color"></div>
                    <span>Generation 4</span>
                </div>
                <div class="legend-badge">
                    <div class="legend-color-box gen-5-color"></div>
                    <span>Generation 5+</span>
                </div>
            </div>
        </div>

        <!-- Tree -->
        <div class="tree-container">
            <ul class="tree-list" id="familyTree"></ul>
        </div>
    </div>

    <script>
        // Family Data (same structure as before)
        const familyData = {
            name: "Mammad Koya",
            spouse: "Paathu & Paathummai",
            generation: 1,
            children: [
                {
                    name: "1. Koya Moideen",
                    spouse: "Ayisha",
                    generation: 2,
                    coordinators: "Masood, Pappan, Suhas",
                    children: [
                        {
                            name: "1.1 Mammed Koya",
                            spouse: "Pathumma",
                            generation: 3,
                            children: [
                                { name: "1.1.1 Mansoor", spouse: "Fareeda", generation: 4, children: "Faiz, Fathima Najah, Aysha, Khadeeja, Maryam" },
                                { name: "1.1.2 Marzook", spouse: "Noorin", generation: 4, children: "Hiba, Aamir, Hazine" },
                                { name: "1.1.3 Masood", spouse: "Faseela", generation: 4, children: "Isra, Afra, Imran" },
                                { name: "1.1.4 Mahroof", spouse: "Jesmina", generation: 4, children: "Eyra Maryam, Adam, Miran" },
                                { name: "1.1.5 Shameeha", spouse: "Jaleel", generation: 4, children: "Ahmed Shefin, Omer Afthab, Rayan" },
                                { name: "1.1.6 Sajida", spouse: "Shejil", generation: 4, children: "Rua Khadeeja" }
                            ]
                        },
                        {
                            name: "1.2 Paathu",
                            spouse: "Hussan Koya",
                            generation: 3,
                            children: [
                                {
                                    name: "1.2.1 Ayishabi",
                                    spouse: "Mayin",
                                    generation: 4,
                                    children: [
                                        { name: "1.2.1.1 Shanavas", spouse: "Shabna", generation: 5, children: "Fathima Nalwa, Aysha Irin" },
                                        { name: "1.2.1.2 Najeebullah", spouse: "Nusreen", generation: 5, children: "Isha Fathima, Eva Fathima" },
                                        { name: "1.2.1.3 Noorudheen", spouse: "Jashra", generation: 5, children: "Sameeha, Emin" },
                                        { name: "1.2.1.4 Abdul Vahab", spouse: "Risna Faijas", generation: 5 }
                                    ]
                                },
                                {
                                    name: "1.2.2 Suhara",
                                    spouse: "Ammad",
                                    generation: 4,
                                    children: [
                                        { name: "1.2.2.1 Jasna", spouse: "Mujeeb", generation: 5, children: "Aysha Haya, Ameen Ahsan, Fathima Amal, Ali Ahsan, Amna Khadeeja" },
                                        { name: "1.2.2.2 Suhaila", spouse: "Thanzeem", generation: 5, children: "Hathim Muhammad" }
                                    ]
                                },
                                {
                                    name: "1.2.3 Musthafa",
                                    spouse: "Hajara",
                                    generation: 4,
                                    children: [
                                        { name: "1.2.3.1 Meha", spouse: "Shareef", generation: 5, children: "Amina Imza, Maryam Aqsa, Aisha Haiza" },
                                        { name: "1.2.3.2 Muziyaf", spouse: "Minana", generation: 5 }
                                    ]
                                },
                                {
                                    name: "1.2.4 Sahida",
                                    spouse: "Musthafa",
                                    generation: 4,
                                    children: [
                                        { name: "1.2.4.1 Fadiya", spouse: "Nabeel", generation: 5, children: "Zidane, Emad, Nooh" },
                                        { name: "1.2.4.2 Farha", spouse: "Shemin", generation: 5, children: "Sulthan, Rakan" },
                                        { name: "1.2.4.3 Falak", spouse: "Fajis", generation: 5, children: "Zenha Fathima" }
                                    ]
                                },
                                {
                                    name: "1.2.5 Hafsa",
                                    spouse: "Muhammad Iqbal",
                                    generation: 4,
                                    children: [
                                        { name: "1.2.5.1 Dilruba", spouse: "Ansar", generation: 5, children: "Ayaan Ahmed, Ehaan Ahmed" },
                                        { name: "1.2.5.2 Mehruba", spouse: "Faseen", generation: 5, children: "Ruhan Shazil" },
                                        { name: "1.2.5.3 Mehbooba", generation: 5 }
                                    ]
                                }
                            ]
                        },
                        {
                            name: "1.3 Asiya",
                            spouse: "Aboobacker",
                            generation: 3,
                            children: [
                                {
                                    name: "1.3.1 Alikkutty",
                                    spouse: "Raseena",
                                    generation: 4,
                                    children: [
                                        { name: "1.3.1.1 Hiba nasrin", spouse: "Niyas", generation: 5, children: [
                                            { name: "1.3.1.1.1 Hyzin muhammed", generation: 5 }
                                        ]},
                                        { name: "1.3.1.2 Nada nasrin", generation: 5 },
                                        { name: "1.3.1.3 Minha", generation: 5 }
                                    ]
                                },
                                {
                                    name: "1.3.2 Asma",
                                    spouse: "Majeed",
                                    generation: 4,
                                    children: [
                                        { name: "1.3.2.1 Jaseena", spouse: "sabeel", generation: 5, children: [
                                            { name: "1.3.2.1.1 Ehan sabeel", generation: 5 },
                                            { name: "1.3.2.1.2 mazin sabeel", generation: 5 }
                                        ]},
                                        { name: "1.3.2.2 Jasil", spouse: "Hiba backar", generation: 5 }
                                    ]
                                },
                                {
                                    name: "1.3.3 Habeeb",
                                    spouse: "Fousiya",
                                    generation: 4,
                                    children: [
                                        { name: "1.3.3.1 Dilshad", generation: 5 },
                                        { name: "1.3.3.2 Dilna", generation: 5 },
                                        { name: "1.3.3.3 Ayisha fildha", generation: 5 }
                                    ]
                                },
                                {
                                    name: "1.3.4 Shameena",
                                    spouse: "Rasheed",
                                    generation: 4,
                                    children: [
                                        { name: "1.3.4.1 Shibnu", generation: 5 },
                                        { name: "1.3.4.2 Sufiyan", generation: 5 },
                                        { name: "1.3.4.3 Ridhwan", generation: 5 }
                                    ]
                                },
                                {
                                    name: "1.3.5 Naseera",
                                    spouse: "Muhammed",
                                    generation: 4,
                                    children: [
                                        { name: "1.3.5.1 Fathima Jumana", spouse: "shafi muhammed", generation: 5, children: [
                                            { name: "1.3.5.1.1 mehra fathima", generation: 5 }
                                        ]},
                                        { name: "1.3.5.2 Humaida Nasrin", generation: 5 },
                                        { name: "1.3.5.3 Munshida", generation: 5 }
                                    ]
                                }
                            ]
                        },
                        {
                            name: "1.4 Sulaiman",
                            spouse: "Safiya",
                            generation: 3,
                            children: [
                                { name: "1.4.1 Sajeer", spouse: "Dilshath", generation: 4, children: "Azlan" }
                            ]
                        },
                        {
                            name: "1.5 Basheer",
                            spouse: "Saara",
                            generation: 3,
                            children: [
                                { name: "1.5.1 Mujeeb", generation: 4 },
                                { name: "1.5.2 Mubeena", spouse: "Musthfa", generation: 4, children: "Minha Fathima, Fathima wifna" },
                                { name: "1.5.3 Mubashira", generation: 4 }
                            ]
                        },
                        {
                            name: "1.6 Ashraf",
                            spouse: "Sabira",
                            generation: 3,
                            children: [
                                { name: "1.6.1 Harshad", spouse: "Ayishasafa", generation: 4, children: "AmeliaRaha" },
                                { name: "1.6.2 Ansab", generation: 4 },
                                { name: "1.6.3 Ashna", spouse: "Shamnas", generation: 4, children: "Thamiz & Ehaan" }
                            ]
                        },
                        {
                            name: "1.7 Saina",
                            spouse: "Muhammed Master",
                            generation: 3,
                            children: [
                                { name: "1.7.1 Muhsina", spouse: "Faisal", generation: 4, children: "Sidan Ahammed, Aisha Faisal & Fathima" },
                                { name: "1.7.2 Aayisha", spouse: "Siddique", generation: 4, children: "FadilMuhammed & Ali Aibak" },
                                { name: "1.7.3 Ameena", spouse: "Riyas", generation: 4, children: "NazalBacker & Nooh" },
                                { name: "1.7.4 Abeeda", spouse: "Muneer", generation: 4, children: "Faizan muhammed, Ivaan Adam & Hamdan" }
                            ]
                        },
                        {
                            name: "1.8 Nafeesa",
                            spouse: "Muhammed Koya",
                            generation: 3,
                            children: [
                                { name: "1.8.1 Siraj", spouse: "Roshin farsana", generation: 4, children: "Yaseen & Thaha, khadeeja masha" },
                                { name: "1.8.2 Suhas", spouse: "Shifana", generation: 4, children: "Afan Muhammad & Anha mariyam" },
                                { name: "1.8.3 Sulaika", spouse: "Subair", generation: 4, children: "junnus & Henna, zidheen ameen" }
                            ]
                        },
                        {
                            name: "1.9 Ramla",
                            spouse: "Majeed",
                            generation: 3,
                            children: [
                                { name: "1.9.1 Rineesh Pappa", spouse: "Sulfath", generation: 4, children: "muhammed Razin & Muhammed Reyyan" },
                                { name: "1.9.2 Manaf", spouse: "Shaikha", generation: 4, children: "muhammed izyan" },
                                { name: "1.9.3 Jiyas", spouse: "Suhana", generation: 4, children: "Emric Abdu" }
                            ]
                        }
                    ]
                },
                {
                    name: "2. Ayisha",
                    spouse: "Koyakkutty Haji",
                    generation: 2,
                    coordinators: "Sadik, Sajid",
                    children: [
                        {
                            name: "2.1 Muhammed (Late)",
                            spouse: "Mariya",
                            generation: 3,
                            children: [
                                { name: "2.1.1 Sabira", spouse: "Latheef", generation: 4, children: "Faseeh, Naseeh and Ramsiya" },
                                { name: "2.1.2 Najma", spouse: "Aboobacker", generation: 4, children: "Mohd Aslam, Amjad and Ahsana" }
                            ]
                        },
                        {
                            name: "2.2 Koyatheen",
                            spouse: "Raheema & Suhara",
                            generation: 3,
                            children: [
                                { name: "2.2.1 Anwar Sadique TK", spouse: "Sajna Tk", generation: 4, children: "Nuha, Nibras and Naifa" },
                                { name: "2.2.2 Anvar Sajid TK", spouse: "Shabna C", generation: 4, children: "Sana fathima, Rozain Sajid and Elzin Sajid" },
                                { name: "2.2.3 Mohd Shafin", spouse: "Jouhara", generation: 4, children: "Mohd Nishan and Afin Roshan" },
                                { name: "2.2.4 Mohd Shanin", spouse: "Jawahara", generation: 4, children: "Mohd Nishal and Benil Afiq" },
                                { name: "2.2.5 Shahin Muhammed T K", spouse: "Amitha Sissil", generation: 4, children: "Aysha Zarrah, Aihan Muhammed T K, and Ayaan Muhammed T K" }
                            ]
                        },
                        {
                            name: "2.3 Abdurahiman (Late)",
                            spouse: "Ayisha",
                            generation: 3,
                            children: [
                                { name: "2.3.1 Sajna", spouse: "Sadique", generation: 4, children: "Nuha, Nibras and Naifa" },
                                { name: "2.3.2 Rajula", spouse: "Basheer", generation: 4, children: "Ridha Fathima and Manu" }
                            ]
                        },
                        {
                            name: "2.4 Kunjirayin",
                            spouse: "Subaida",
                            generation: 3,
                            children: [
                                { name: "2.4.1 Musthafa", spouse: "Thanzeela", generation: 4, children: "Aiza fathma, Azah Ayrin" },
                                { name: "2.4.2 Latheef", spouse: "Aysha Sulfath", generation: 4, children: "Aibak Razi, Aysh Hamd" },
                                { name: "2.4.3 Muhsina", spouse: "Masood", generation: 4, children: "Mahveen Mariyam" }
                            ]
                        },
                        {
                            name: "2.5 Aboobakker",
                            spouse: "Souda",
                            generation: 3,
                            children: [
                                { name: "2.5.1 Jilsana", spouse: "Muneer TP", generation: 4, children: "Fathima Najah Muneer, and Minha" },
                                { name: "2.5.2 Jirshana", spouse: "Ilthumish P", generation: 4, children: "Shamil MK and Shayan MK" }
                            ]
                        },
                        {
                            name: "2.6 Nafeesa",
                            spouse: "Bakkar",
                            generation: 3,
                            children: [
                                { name: "2.6.1 Soudha", spouse: "Mujeeb", generation: 4, children: "Basima, and Minu" },
                                { name: "2.6.2 Mujeeb", spouse: "Rahmath", generation: 4, children: "Nida, Rinu and Mihras" },
                                { name: "2.6.3 Riyas", spouse: "Asna", generation: 4, children: "Sayan, Rayyan and Liban" },
                                { name: "2.6.4 Fasna", spouse: "Faisal", generation: 4, children: "Mehbin, Miyan and Meyana" }
                            ]
                        },
                        {
                            name: "2.7 Musthafa",
                            spouse: "Soudha",
                            generation: 3,
                            children: [
                                { name: "2.7.1 Ameera", spouse: "Noufal", generation: 4, children: "Nina kenz and Niza kenz" },
                                { name: "2.7.2 Shaheem", spouse: "Farsana mp", generation: 4, children: "Faliq Zaman TK" },
                                { name: "2.7.3 Rajeeb", spouse: "Aakhila", generation: 4 },
                                { name: "2.7.4 Ayisha", spouse: "Shabas", generation: 4, children: "Ahil and Aban" }
                            ]
                        },
                        {
                            name: "2.8 Subaida",
                            spouse: "Aseez",
                            generation: 3,
                            children: [
                                { name: "2.8.1 Shahina", spouse: "Saleem", generation: 4, children: "Khadin Sahir, Riya Raha and Rayan Muhammed" },
                                { name: "2.8.2 Haseena", spouse: "Sadath", generation: 4, children: "Fathima Minha, Misna fathima and Emlah Yezra" },
                                { name: "2.8.3 Asharudheen", spouse: "Muhsina", generation: 4, children: "Iza Fathima and Verza" },
                                { name: "2.8.4 Shasudheen", spouse: "Safna Sherin", generation: 4, children: "Mohd Ayan" }
                            ]
                        }
                    ]
                },
                {
                    name: "3. Abdurahiman Kutty",
                    spouse: "Amina",
                    generation: 2,
                    coordinators: "Vaavatha, Chittu",
                    children: [
                        {
                            name: "3.1 Paathu",
                            spouse: "Muneer",
                            generation: 3,
                            children: [
                                { name: "3.1.1 Deeja", spouse: "Late Hassan Koya", generation: 4, children: "Multiple children including Sansi Hassan, Shekha Sheri" },
                                { name: "3.1.2 Meena", spouse: "Hameed", generation: 4, children: "Leniyah Loola, Dervish Hussain" },
                                { name: "3.1.3 Riya", spouse: "Rasheed", generation: 4, children: "Abhlah Khadeeja & Mazen Muhammed" },
                                { name: "3.1.4 Mufasir", spouse: "Norhaina", generation: 4, children: "Hamad, Hamdan, Hammer, Hamran, Hamjaan, Hamzaan, Hamera Fathima" }
                            ]
                        },
                        {
                            name: "3.2 Koya",
                            spouse: "Subaida",
                            generation: 3,
                            children: [
                                { name: "3.2.1 Shameek", spouse: "Farisha", generation: 4, children: "Alen Airik" },
                                { name: "3.2.2 Shabna", spouse: "Sakeer", generation: 4, children: "Muhammed Sinan & Ayisha Zenha" },
                                { name: "3.2.3 Sajna", spouse: "Hisham", generation: 4, children: "Minza Fathima, Aiza Fathima & Muhammed Zayan" }
                            ]
                        },
                        {
                            name: "3.3 Aseez",
                            spouse: "Noorunnisa",
                            generation: 3,
                            children: [
                                { name: "3.3.1 Sharbi", spouse: "Haris", generation: 4, children: "Fadhi Hanan, Zain Humdhan & Fezin Hanik" },
                                { name: "3.3.2 Shahanas", spouse: "Muhammed Koya", generation: 4, children: "Sheza Fathima, Ali Miyan, Thaish Ahamed" },
                                { name: "3.3.3 Shahanoof", spouse: "Sajeeha", generation: 4, children: "Tahnoun Mohammed" }
                            ]
                        },
                        {
                            name: "3.4 Souja EK",
                            spouse: "Mammadkoya",
                            generation: 3,
                            children: [
                                { name: "3.4.1 Jasmine", spouse: "mirshaad", generation: 4, children: "safarul marjaan & safarul minhaaj" },
                                { name: "3.4.2 Jamsheer", spouse: "jasniya", generation: 4, children: "minza fathima & Muhammed jasim" },
                                { name: "3.4.3 Jasheer", spouse: "Haseelath", generation: 4, children: "Hadiya fathima, Muhammed aizeen, Muhammed faizeen" },
                                { name: "3.4.4 Jasir", spouse: "Fida Parvin", generation: 4, children: "Muhammed Al Rihlan" },
                                { name: "3.4.5 Jasna", spouse: "Abdul Harisha", generation: 4, children: "Dhanish, Muhammed Hayan, Muhammed Haidaan" }
                            ]
                        },
                        {
                            name: "3.5 Rasiya",
                            spouse: "Kuttimammy",
                            generation: 3,
                            children: [
                                { name: "3.5.1 Shajudheen", spouse: "Zoya", generation: 4, children: "Amina Niza & Muhammed Eshan" },
                                { name: "3.5.2 Sainudheen", spouse: "Sabira", generation: 4, children: "Shenza Thaniya & Shenzil Faizan" }
                            ]
                        },
                        {
                            name: "3.6 Abdullakkoya",
                            spouse: "Hajara",
                            generation: 3,
                            children: [
                                { name: "3.6.1 Ajnas", spouse: "Narjas", generation: 4, children: "Nashwa Mehrin & Nahan Ayman" },
                                { name: "3.6.2 Ajeeb", spouse: "Nafeesathul Misriya", generation: 4 },
                                { name: "3.6.3 Ajmal farveena", spouse: "Aris", generation: 4, children: "Ayisha Faiha & Muhammed faizan" }
                            ]
                        }
                    ]
                },
                {
                    name: "4. Hassan",
                    spouse: "Imbichipathu & Paathu",
                    generation: 2,
                    coordinators: "Rafi",
                    children: [
                        {
                            name: "4.1 Mammadkoya",
                            spouse: "Subaida",
                            generation: 3,
                            children: [
                                { name: "4.1.1 Mirshad", spouse: "Aneesha", generation: 4, children: "Muhammed Afraz, Emil Mehzan" },
                                { name: "4.1.2 Shahana", spouse: "Jamsheer", generation: 4, children: "Ayisha Lamha, Fathima Haala" },
                                { name: "4.1.3 Thasna", spouse: "Muhammed Sadique", generation: 4, children: "Jafakkash, Iffah Meiz, Rooha Meiz" }
                            ]
                        },
                        {
                            name: "4.2 Sakeer",
                            spouse: "Maimoonath",
                            generation: 3,
                            children: [
                                { name: "4.2.1 Mohd Shafi", spouse: "Febin Rasheed", generation: 4, children: "Shan Aybak, Abel Fathin" },
                                { name: "4.2.2 Mohd Rafi", spouse: "Muhsina", generation: 4, children: "Imad Hassan, llan Malik" },
                                { name: "4.2.3 Shakira", spouse: "Faisal", generation: 4, children: "Faiza Fathima, Dua Mariyam, Inam Faisal" }
                            ]
                        },
                        {
                            name: "4.3 Saleena",
                            spouse: "Abdulla",
                            generation: 3,
                            children: [
                                { name: "4.3.1 Nasleena", spouse: "Sameer Fizan", generation: 4 },
                                { name: "4.3.2 Nisham", spouse: "Munsila", generation: 4, children: "Wildan Adam" }
                            ]
                        }
                    ]
                },
                {
                    name: "5. Sulaiman",
                    spouse: "Paathay",
                    generation: 2,
                    coordinators: "Sulfath, Shibili",
                    children: [
                        {
                            name: "5.1 Nafeesa",
                            spouse: "Abdurahiman",
                            generation: 3,
                            children: [
                                { name: "5.1.1 Shibili", spouse: "Muneer", generation: 4, children: "Sanan, Diyan" },
                                { name: "5.1.2 Shabna", spouse: "Jamsheer", generation: 4, children: "Shibin Hassan, Afra, Mariyam" },
                                { name: "5.1.3 Shabil", spouse: "Merlin", generation: 4 }
                            ]
                        },
                        {
                            name: "5.2 Subaida",
                            spouse: "Abdulla",
                            generation: 3,
                            children: [
                                { name: "5.2.1 Nusrath", spouse: "Abdul Gafoor", generation: 4, children: "Adil, Aysha, Ahadiah" },
                                { name: "5.2.2 Sulfath", spouse: "Sanith", generation: 4, children: "Naiza Mariyam, Shaid sulaiman" },
                                { name: "5.2.3 Dayana", spouse: "Suhail", generation: 4, children: "Tanisha Fathima" }
                            ]
                        },
                        {
                            name: "5.3 Rasheed",
                            spouse: "Subaida",
                            generation: 3,
                            children: [
                                { name: "5.3.1 Rejin Rasheed", spouse: "Dilshana", generation: 4, children: "Liya Fathima, Amana Mariyam" },
                                { name: "5.3.2 Rajeena", spouse: "Dilsar", generation: 4, children: "Isha Mehara, Diya Fathima" }
                            ]
                        },
                        {
                            name: "5.4 Shareefa",
                            generation: 3,
                            children: [
                                { name: "5.4.1 Annath", spouse: "shajahan", generation: 4, children: "Minhaj, Midlaj" },
                                { name: "5.4.2 Jamsheer", generation: 4 }
                            ]
                        }
                    ]
                },
                {
                    name: "6. Kunjiperi Haji",
                    spouse: "Kadeeja & Suleikha",
                    generation: 2,
                    coordinators: "Aaqib, Sini",
                    children: [
                        {
                            name: "6.1 Latheef",
                            spouse: "Zulekha",
                            generation: 3,
                            children: [
                                { name: "6.1.1 Kadeeja", spouse: "Jawadh", generation: 4, children: "Ziram, Tahani" },
                                { name: "6.1.2 Aaqib", spouse: "Mifra", generation: 4, children: "Amiq" },
                                { name: "6.1.3 Tayyib", generation: 4 }
                            ]
                        },
                        {
                            name: "6.2 Musthafa",
                            spouse: "Rajeena",
                            generation: 3,
                            children: [
                                { name: "6.2.1 Fathima", spouse: "Asvakh", generation: 4, children: "Zenha, Ziya" },
                                { name: "6.2.2 Akheel", spouse: "Hana", generation: 4 },
                                { name: "6.2.3 Amar", generation: 4 }
                            ]
                        },
                        {
                            name: "6.3 Jameela",
                            spouse: "Nazeer",
                            generation: 3,
                            children: [
                                { name: "6.3.1 Shamna", spouse: "Asif", generation: 4, children: "Aydin" },
                                { name: "6.3.2 Aqthar", generation: 4 },
                                { name: "6.3.3 Afthab", generation: 4 }
                            ]
                        }
                    ]
                },
                {
                    name: "7. Moideen",
                    spouse: "Aamina",
                    generation: 2,
                    coordinators: "Manaf, Safwan",
                    children: [
                        {
                            name: "7.1 Razak",
                            spouse: "Naseema",
                            generation: 3,
                            children: [
                                { name: "7.1.1 Manaf", spouse: "shabana", generation: 4, children: "Raif Halim, Inarah khadeeja" },
                                { name: "7.1.2 Minhaj", spouse: "shahana", generation: 4, children: "Haniya mariyam" },
                                { name: "7.1.3 Muneer", spouse: "Ashila", generation: 4 }
                            ]
                        },
                        {
                            name: "7.2 Kabeer",
                            spouse: "Sainaba",
                            generation: 3,
                            children: [
                                { name: "7.2.1 Fasal", spouse: "Najiya Nasrin", generation: 4, children: "Aymen Emaad, Amish Ezlaan" },
                                { name: "7.2.2 Fayis", spouse: "Fathima Rifa", generation: 4 }
                            ]
                        },
                        {
                            name: "7.3 Fathima",
                            spouse: "Seyid Muhammed",
                            generation: 3,
                            children: [
                                { name: "7.3.1 Sharfas", spouse: "Roshna", generation: 4, children: "Fathima Faiqah, Ehan Muhammed" },
                                { name: "7.3.2 Safwan", spouse: "Liyana", generation: 4, children: "Inaya safwan" },
                                { name: "7.3.3 Shafana", spouse: "Junaid", generation: 4, children: "Zama mehak" }
                            ]
                        }
                    ]
                },
                {
                    name: "8. Kunjayin",
                    spouse: "Sainaba",
                    generation: 2,
                    coordinators: "Kunjol",
                    children: [
                        {
                            name: "8.1 Rasleena",
                            spouse: "Hus",
                            generation: 3,
                            children: [
                                { name: "8.1.1 Ayisha Limtha", spouse: "Shaheen", generation: 4, children: "Elah" },
                                { name: "8.1.2 Mohd Aman", generation: 4 },
                                { name: "8.1.3 Isha Mahbin", generation: 4 }
                            ]
                        },
                        {
                            name: "8.2 Salman",
                            spouse: "Roshna",
                            generation: 3,
                            children: [
                                { name: "8.2.1 Aybak", generation: 4 }
                            ]
                        }
                    ]
                },
                {
                    name: "9. Aasiya",
                    spouse: "Muhammed",
                    generation: 2,
                    coordinators: "Kuttan, Kunjol",
                    children: []
                }
            ]
        };

        function getInitials(name) {
            return name.split(' ').slice(0, 2).map(n => n[0]).join('').toUpperCase();
        }

        function renderNode(node, isExpanded = false) {
            const hasChildren = node.children && (Array.isArray(node.children) ? node.children.length > 0 : node.children);
            const nodeId = 'node-' + Math.random().toString(36).substr(2, 9);
            
            let html = '<li class="tree-node" data-node-id="' + nodeId + '">';
            
            // Member Card
            html += '<div class="member-card gen-' + node.generation + '-card" onclick="toggleNode(\'' + nodeId + '\')">';
            html += '<div class="member-avatar">' + getInitials(node.name) + '</div>';
            html += '<div class="member-info">';
            html += '<div class="member-name">' + node.name + '</div>';
            
            if (node.spouse) {
                html += '<div class="member-spouse">';
                html += '<span class="marriage-icon">✦</span> ' + node.spouse;
                html += '</div>';
            }
            
            html += '</div>';
            
            if (hasChildren) {
                html += '<div class="expand-indicator">' + (isExpanded ? '−' : '+') + '</div>';
            }
            
            html += '<span class="gen-badge">Gen ' + node.generation + '</span>';
            html += '</div>';
            
            // Coordinator Badge
            if (node.coordinators) {
                html += '<div class="coordinator-badge">';
                html += '<span class="coordinator-icon">📋</span>';
                html += '<span>Coordinators: ' + node.coordinators + '</span>';
                html += '</div>';
            }
            
            // Children
            if (hasChildren) {
                html += '<ul class="children-container' + (isExpanded ? ' expanded' : '') + '" id="children-' + nodeId + '">';
                
                if (Array.isArray(node.children)) {
                    node.children.forEach(child => {
                        html += renderNode(child, isExpanded);
                    });
                } else if (typeof node.children === 'string') {
                    html += '<li class="children-list">' + node.children + '</li>';
                }
                
                html += '</ul>';
            }
            
            html += '</li>';
            return html;
        }

        function toggleNode(nodeId) {
            const childrenEl = document.getElementById('children-' + nodeId);
            const cardEl = document.querySelector('[data-node-id="' + nodeId + '"] .member-card');
            const indicator = cardEl.querySelector('.expand-indicator');
            
            if (childrenEl) {
                childrenEl.classList.toggle('expanded');
                indicator.textContent = childrenEl.classList.contains('expanded') ? '−' : '+';
            }
        }

        function expandAll() {
            document.querySelectorAll('.children-container').forEach(el => el.classList.add('expanded'));
            document.querySelectorAll('.expand-indicator').forEach(el => el.textContent = '−');
        }

        function collapseAll() {
            document.querySelectorAll('.children-container').forEach(el => el.classList.remove('expanded'));
            document.querySelectorAll('.expand-indicator').forEach(el => el.textContent = '+');
        }

        function searchFamily() {
            const searchTerm = document.getElementById('searchInput').value.toLowerCase().trim();
            
            if (!searchTerm) {
                alert('Please enter a search term');
                return;
            }
            
            document.querySelectorAll('.member-card').forEach(el => el.classList.remove('highlighted'));
            
            const allCards = document.querySelectorAll('.member-name, .member-spouse');
            let foundCount = 0;
            
            allCards.forEach(el => {
                if (el.textContent.toLowerCase().includes(searchTerm)) {
                    foundCount++;
                    const card = el.closest('.member-card');
                    card.classList.add('highlighted');
                    
                    let parent = card.closest('.children-container');
                    while (parent) {
                        parent.classList.add('expanded');
                        const parentCard = parent.previousElementSibling;
                        if (parentCard && parentCard.classList.contains('member-card')) {
                            const indicator = parentCard.querySelector('.expand-indicator');
                            if (indicator) indicator.textContent = '−';
                        }
                        parent = parent.parentElement.closest('.children-container');
                    }
                    
                    if (foundCount === 1) {
                        card.scrollIntoView({ behavior: 'smooth', block: 'center' });
                    }
                }
            });
            
            if (foundCount === 0) {
                alert('No results found for "' + searchTerm + '"');
            } else {
                alert('Found ' + foundCount + ' result(s)');
            }
        }

        function clearSearch() {
            document.getElementById('searchInput').value = '';
            document.querySelectorAll('.member-card').forEach(el => el.classList.remove('highlighted'));
            collapseAll();
        }

        function initTree() {
            const container = document.getElementById('familyTree');
            container.innerHTML = renderNode(familyData, false);
        }

        document.addEventListener('DOMContentLoaded', function() {
            initTree();
            
            document.getElementById('searchInput').addEventListener('keypress', function(e) {
                if (e.key === 'Enter') searchFamily();
            });
        });
    </script>
</body>
</html>
