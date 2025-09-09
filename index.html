<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Royal Poker Club - Seat Booking</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
        
        body {
            font-family: 'Inter', sans-serif;
            background: linear-gradient(135deg, #0f172a 0%, #1e293b 25%, #334155 50%, #1e293b 75%, #0f172a 100%);
            min-height: 100vh;
        }
        
        .poker-bg {
            background-image: 
                radial-gradient(circle at 20% 20%, rgba(255, 215, 0, 0.08) 0%, transparent 50%),
                radial-gradient(circle at 80% 80%, rgba(34, 197, 94, 0.06) 0%, transparent 50%),
                radial-gradient(circle at 40% 60%, rgba(59, 130, 246, 0.05) 0%, transparent 50%),
                radial-gradient(circle at 60% 20%, rgba(239, 68, 68, 0.04) 0%, transparent 50%);
        }
        
        .card-shadow {
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.5), 0 10px 10px -5px rgba(0, 0, 0, 0.3);
        }
        
        .poker-chip {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: conic-gradient(from 0deg, #ef4444, #f97316, #eab308, #22c55e, #3b82f6, #8b5cf6, #ef4444);
            display: inline-block;
            margin: 0 5px;
            animation: spin 10s linear infinite;
        }
        
        @keyframes spin {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }
        
        .suit-symbol {
            font-size: 2rem;
            opacity: 0.1;
            position: absolute;
            animation: float 6s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
        }
        
        .hidden { display: none !important; }
        .show { display: block !important; }
        
        /* Loading spinner */
        .loading-spinner {
            border: 4px solid #f3f3f3;
            border-top: 4px solid #3498db;
            border-radius: 50%;
            width: 50px;
            height: 50px;
            animation: spin 2s linear infinite;
            margin: 20px auto;
        }
        
        /* Ensure content is visible */
        .main-content {
            opacity: 1;
            transition: opacity 0.3s ease-in-out;
        }
    </style>
</head>
<body class="poker-bg">
    <!-- Loading indicator -->
    <div id="loadingIndicator" class="fixed inset-0 bg-gray-900 flex items-center justify-center z-50" style="display: none;">
        <div class="text-center">
            <div class="loading-spinner"></div>
            <p class="text-white mt-4">Loading 10K Clubhouse...</p>
        </div>
    </div>

    <div class="main-content">
        <!-- Floating poker symbols -->
        <div class="suit-symbol text-yellow-400" style="top: 10%; left: 5%; animation-delay: 0s;">♠</div>
        <div class="suit-symbol text-red-500" style="top: 20%; right: 10%; animation-delay: 1s;">♥</div>
        <div class="suit-symbol text-yellow-400" style="top: 60%; left: 8%; animation-delay: 2s;">♦</div>
        <div class="suit-symbol text-gray-400" style="top: 80%; right: 15%; animation-delay: 3s;">♣</div>
        <div class="suit-symbol text-red-500" style="top: 40%; left: 85%; animation-delay: 4s;">♠</div>

        <div class="container mx-auto px-4 py-8">
            <!-- Header -->
            <header class="text-center mb-12">
                <h1 class="text-5xl font-bold text-yellow-300 mb-4 drop-shadow-lg">
                    🏆 10K Clubhouse 🏆
                </h1>
                <p class="text-xl text-gray-300">Premium Poker Experience • Baccarat Royale • Secure Reservations</p>
            </header>

            <!-- Navigation -->
            <nav class="flex justify-between items-center mb-8">
                <div class="bg-black/60 backdrop-blur-sm rounded-full p-2 border border-gray-700">
                    <button onclick="showSection('booking')" id="bookingBtn" class="px-6 py-3 rounded-full bg-blue-600 text-white font-medium mx-2 transition-all">
                        💎 Book Seat
                    </button>
                    <button onclick="showSection('schedule')" id="scheduleBtn" class="px-6 py-3 rounded-full text-gray-300 hover:bg-gray-700 font-medium mx-2 transition-all">
                        🗓️ Schedule
                    </button>
                </div>
                
                <!-- Login/User Section -->
                <div class="flex items-center space-x-4">
                    <!-- User Info (when logged in) -->
                    <div id="userInfo" class="hidden bg-black/60 backdrop-blur-sm rounded-full px-4 py-2 border border-gray-700">
                        <div class="flex items-center space-x-3">
                            <div id="userAvatar" class="w-8 h-8 rounded-full bg-blue-600 flex items-center justify-center text-white font-bold text-sm">
                                A
                            </div>
                            <div>
                                <p id="userName" class="text-white font-medium text-sm">Admin User</p>
                                <p id="userRole" class="text-gray-400 text-xs">Administrator</p>
                            </div>
                            <button onclick="logout()" class="text-red-400 hover:text-red-300 text-sm ml-2">
                                🚪 Logout
                            </button>
                        </div>
                    </div>
                    
                    <!-- Login Button -->
                    <button onclick="showLoginModal()" id="loginBtn" class="bg-gradient-to-r from-purple-600 to-purple-700 hover:from-purple-700 hover:to-purple-800 text-white font-bold px-6 py-3 rounded-full transition-all">
                        🔑 Login
                    </button>
                </div>
            </nav>

            <!-- Booking Section -->
            <section id="bookingSection" class="max-w-4xl mx-auto">
                <div class="bg-black/40 backdrop-blur-sm rounded-2xl p-8 card-shadow border border-gray-600">
                    <h2 class="text-3xl font-bold text-white mb-8 text-center">💺 Reserve Your Seat</h2>
                    
                    <form id="bookingForm" class="grid md:grid-cols-2 gap-8">
                        <div class="space-y-6">
                            <div>
                                <label class="block text-gray-300 font-medium mb-2">Player Name</label>
                                <input type="text" id="playerName" class="w-full p-4 bg-gray-800/70 border border-gray-600 rounded-xl text-white focus:border-blue-500 focus:outline-none" placeholder="Enter your name" required readonly>
                                <p class="text-gray-400 text-xs mt-1">🔒 Login required to auto-fill your registered name</p>
                            </div>
                            
                            <div>
                                <label class="block text-gray-300 font-medium mb-2">Phone Number</label>
                                <input type="tel" id="playerPhone" class="w-full p-4 bg-gray-800/70 border border-gray-600 rounded-xl text-white focus:border-blue-500 focus:outline-none" placeholder="+60 12-345 6789" required>
                            </div>
                            
                            <div>
                                <label class="block text-gray-300 font-medium mb-2">Referring Agent (Optional)</label>
                                <select id="referringAgent" class="w-full p-4 bg-gray-800/70 border border-gray-600 rounded-xl text-white focus:border-blue-500 focus:outline-none">
                                    <option value="">Select Agent</option>
                                    <option value="agent1">Mike Chen</option>
                                    <option value="agent2">Sarah Johnson</option>
                                    <option value="agent3">David Rodriguez</option>
                                    <option value="agent4">Lisa Wang</option>
                                </select>
                            </div>
                        </div>
                        
                        <div class="space-y-6">
                            <div>
                                <label class="block text-gray-300 font-medium mb-2">Scheduled Game Session</label>
                                <select id="gameSession" class="w-full p-4 bg-gray-800/70 border border-gray-600 rounded-xl text-white focus:border-blue-500 focus:outline-none" required>
                                    <option value="">Select Game Session</option>
                                </select>
                            </div>
                            
                            <div>
                                <label class="block text-gray-300 font-medium mb-2">Estimated Arrival Time</label>
                                <select id="gameTime" class="w-full p-4 bg-gray-800/70 border border-gray-600 rounded-xl text-white focus:border-blue-500 focus:outline-none" required>
                                    <option value="">Select Arrival Time</option>
                                    <option value="same">Same as Game Start Time</option>
                                    <option value="15min">15 minutes after start</option>
                                    <option value="30min">30 minutes after start</option>
                                    <option value="1hour">1 hour after start</option>
                                </select>
                            </div>
                            
                            <div>
                                <label class="block text-gray-300 font-medium mb-2">Reserve Seat (Optional)</label>
                                <select id="seatReservation" class="w-full p-4 bg-gray-800/70 border border-gray-600 rounded-xl text-white focus:border-blue-500 focus:outline-none" disabled>
                                    <option value="">🔒 Login required to reserve seats</option>
                                    <option value="none">No seat reservation is required</option>
                                    <option value="25_2">Seat 2 - RM 25 💳</option>
                                    <option value="25_3">Seat 3 - RM 25 💳</option>
                                    <option value="25_4">Seat 4 - RM 25 💳</option>
                                    <option value="25_5">Seat 5 - RM 25 💳</option>
                                    <option value="25_6">Seat 6 - RM 25 💳</option>
                                    <option value="25_7">Seat 7 - RM 25 💳</option>
                                    <option value="25_8">Seat 8 - RM 25 💳</option>
                                    <option value="25_9">Seat 9 - RM 25 💳</option>
                                    <option value="25_10">Seat 10 - RM 25 💳</option>
                                </select>
                                <p class="text-gray-400 text-xs mt-1">🔒 Member login required for seat reservations</p>
                                
                                <!-- Reservation Fee Reminder -->
                                <div id="reservationReminder" class="hidden mt-3 p-3 bg-gradient-to-r from-yellow-600/20 to-yellow-800/20 rounded-lg border border-yellow-500/30">
                                    <div class="flex items-center space-x-2">
                                        <span class="text-2xl">🎰</span>
                                        <div>
                                            <p class="text-yellow-300 font-medium text-sm">💰 Reservation Fee Return</p>
                                            <p class="text-yellow-200 text-xs">Your RM 25 reservation fee will be returned as chips upon arrival at the table!</p>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            
                            <div>
                                <label class="block text-gray-300 font-medium mb-2">Food Order (Optional)</label>
                                <textarea id="foodOrder" class="w-full p-4 bg-gray-800/70 border border-gray-600 rounded-xl text-white focus:border-blue-500 focus:outline-none" rows="3" placeholder="Enter your food order here (e.g., Nasi Lemak, Teh Tarik, etc.)"></textarea>
                                <p class="text-gray-400 text-xs mt-1">🍽️ Food will be prepared around your estimated arrival time</p>
                            </div>
                                <div id="paymentSection" class="hidden mt-4 p-4 bg-gradient-to-r from-green-600/20 to-green-800/20 rounded-xl border border-green-500/30">
                                    <h4 class="text-green-300 font-bold mb-3">💳 Choose Payment Method</h4>
                                    
                                    <!-- Payment Method Selection -->
                                    <div class="mb-4">
                                        <div class="grid grid-cols-2 md:grid-cols-4 gap-3">
                                            <button type="button" onclick="selectPaymentMethod('tng')" id="tngBtn" class="payment-method-btn bg-blue-600/30 border-2 border-blue-500 p-3 rounded-lg text-center transition-all hover:bg-blue-600/50">
                                                <div class="text-2xl mb-1">📱</div>
                                                <div class="text-xs text-blue-300 font-medium">Touch 'n Go</div>
                                            </button>
                                            <button type="button" onclick="selectPaymentMethod('grabpay')" id="grabpayBtn" class="payment-method-btn bg-gray-600/30 border-2 border-gray-500 p-3 rounded-lg text-center transition-all hover:bg-gray-600/50">
                                                <div class="text-2xl mb-1">🚗</div>
                                                <div class="text-xs text-gray-300 font-medium">GrabPay</div>
                                            </button>
                                            <button type="button" onclick="selectPaymentMethod('boost')" id="boostBtn" class="payment-method-btn bg-gray-600/30 border-2 border-gray-500 p-3 rounded-lg text-center transition-all hover:bg-gray-600/50">
                                                <div class="text-2xl mb-1">🚀</div>
                                                <div class="text-xs text-gray-300 font-medium">Boost</div>
                                            </button>
                                            <button type="button" onclick="selectPaymentMethod('card')" id="cardBtn" class="payment-method-btn bg-gray-600/30 border-2 border-gray-500 p-3 rounded-lg text-center transition-all hover:bg-gray-600/50">
                                                <div class="text-2xl mb-1">💳</div>
                                                <div class="text-xs text-gray-300 font-medium">Credit Card</div>
                                            </button>
                                        </div>
                                    </div>

                                    <!-- Touch 'n Go Payment -->
                                    <div id="tngPayment" class="payment-form hidden">
                                        <div class="bg-blue-600/20 rounded-lg p-4 mb-4 border border-blue-500/30">
                                            <div class="flex items-center justify-between mb-3">
                                                <div class="flex items-center space-x-3">
                                                    <div class="text-3xl">📱</div>
                                                    <div>
                                                        <h5 class="text-blue-300 font-bold">Touch 'n Go eWallet</h5>
                                                        <p class="text-blue-200 text-sm">Instant & Secure Payment</p>
                                                    </div>
                                                </div>
                                                <div class="text-right">
                                                    <p class="text-blue-300 font-bold text-lg">RM 25.00</p>
                                                </div>
                                            </div>
                                            <div class="bg-white/10 rounded-lg p-3 mb-3">
                                                <p class="text-blue-200 text-sm mb-2">📞 <strong>Transfer to:</strong></p>
                                                <p class="text-white font-mono text-lg">010-300-6940</p>
                                                <p class="text-blue-200 text-xs mt-1">10K Clubhouse Official Account</p>
                                            </div>
                                            <div class="space-y-3">
                                                <div>
                                                    <label class="block text-blue-300 text-sm mb-1">Your Touch 'n Go Phone Number</label>
                                                    <input type="tel" id="tngPhone" class="w-full p-3 bg-gray-700/50 border border-blue-500 rounded-lg text-white focus:border-blue-400 focus:outline-none" placeholder="01X-XXX-XXXX" required>
                                                </div>
                                                <div>
                                                    <label class="block text-blue-300 text-sm mb-1">Transaction Reference ID</label>
                                                    <input type="text" id="tngRef" class="w-full p-3 bg-gray-700/50 border border-blue-500 rounded-lg text-white focus:border-blue-400 focus:outline-none" placeholder="Enter TnG transaction ID after payment" required>
                                                </div>
                                            </div>
                                        </div>
                                    </div>

                                    <!-- GrabPay Payment -->
                                    <div id="grabpayPayment" class="payment-form hidden">
                                        <div class="bg-green-600/20 rounded-lg p-4 mb-4 border border-green-500/30">
                                            <div class="flex items-center justify-between mb-3">
                                                <div class="flex items-center space-x-3">
                                                    <div class="text-3xl">🚗</div>
                                                    <div>
                                                        <h5 class="text-green-300 font-bold">GrabPay</h5>
                                                        <p class="text-green-200 text-sm">Pay with Grab Wallet</p>
                                                    </div>
                                                </div>
                                                <div class="text-right">
                                                    <p class="text-green-300 font-bold text-lg">RM 25.00</p>
                                                </div>
                                            </div>
                                            <div class="bg-white/10 rounded-lg p-3 mb-3">
                                                <p class="text-green-200 text-sm mb-2">📞 <strong>Transfer to:</strong></p>
                                                <p class="text-white font-mono text-lg">010-300-6940</p>
                                                <p class="text-green-200 text-xs mt-1">10K Clubhouse Official Account</p>
                                            </div>
                                            <div class="space-y-3">
                                                <div>
                                                    <label class="block text-green-300 text-sm mb-1">Your GrabPay Phone Number</label>
                                                    <input type="tel" id="grabPhone" class="w-full p-3 bg-gray-700/50 border border-green-500 rounded-lg text-white focus:border-green-400 focus:outline-none" placeholder="01X-XXX-XXXX" required>
                                                </div>
                                                <div>
                                                    <label class="block text-green-300 text-sm mb-1">Transaction Reference ID</label>
                                                    <input type="text" id="grabRef" class="w-full p-3 bg-gray-700/50 border border-green-500 rounded-lg text-white focus:border-green-400 focus:outline-none" placeholder="Enter GrabPay transaction ID" required>
                                                </div>
                                            </div>
                                        </div>
                                    </div>

                                    <!-- Boost Payment -->
                                    <div id="boostPayment" class="payment-form hidden">
                                        <div class="bg-purple-600/20 rounded-lg p-4 mb-4 border border-purple-500/30">
                                            <div class="flex items-center justify-between mb-3">
                                                <div class="flex items-center space-x-3">
                                                    <div class="text-3xl">🚀</div>
                                                    <div>
                                                        <h5 class="text-purple-300 font-bold">Boost</h5>
                                                        <p class="text-purple-200 text-sm">Pay with Boost App</p>
                                                    </div>
                                                </div>
                                                <div class="text-right">
                                                    <p class="text-purple-300 font-bold text-lg">RM 25.00</p>
                                                </div>
                                            </div>
                                            <div class="bg-white/10 rounded-lg p-3 mb-3">
                                                <p class="text-purple-200 text-sm mb-2">📞 <strong>Transfer to:</strong></p>
                                                <p class="text-white font-mono text-lg">010-300-6940</p>
                                                <p class="text-purple-200 text-xs mt-1">10K Clubhouse Official Account</p>
                                            </div>
                                            <div class="space-y-3">
                                                <div>
                                                    <label class="block text-purple-300 text-sm mb-1">Your Boost Phone Number</label>
                                                    <input type="tel" id="boostPhone" class="w-full p-3 bg-gray-700/50 border border-purple-500 rounded-lg text-white focus:border-purple-400 focus:outline-none" placeholder="01X-XXX-XXXX" required>
                                                </div>
                                                <div>
                                                    <label class="block text-purple-300 text-sm mb-1">Transaction Reference ID</label>
                                                    <input type="text" id="boostRef" class="w-full p-3 bg-gray-700/50 border border-purple-500 rounded-lg text-white focus:border-purple-400 focus:outline-none" placeholder="Enter Boost transaction ID" required>
                                                </div>
                                            </div>
                                        </div>
                                    </div>

                                    <!-- Credit Card Payment -->
                                    <div id="cardPayment" class="payment-form hidden">
                                        <div class="bg-yellow-600/20 rounded-lg p-4 mb-4 border border-yellow-500/30">
                                            <h5 class="text-yellow-300 font-bold mb-3">💳 Credit/Debit Card</h5>
                                            <div class="grid md:grid-cols-2 gap-4">
                                                <div>
                                                    <label class="block text-yellow-300 text-sm mb-1">Card Number</label>
                                                    <input type="text" id="cardNumber" class="w-full p-3 bg-gray-600/50 border border-yellow-500 rounded-lg text-white focus:border-yellow-400 focus:outline-none" placeholder="1234 5678 9012 3456" maxlength="19">
                                                </div>
                                                <div>
                                                    <label class="block text-yellow-300 text-sm mb-1">Cardholder Name</label>
                                                    <input type="text" id="cardName" class="w-full p-3 bg-gray-600/50 border border-yellow-500 rounded-lg text-white focus:border-yellow-400 focus:outline-none" placeholder="John Doe">
                                                </div>
                                                <div>
                                                    <label class="block text-yellow-300 text-sm mb-1">Expiry Date</label>
                                                    <input type="text" id="cardExpiry" class="w-full p-3 bg-gray-600/50 border border-yellow-500 rounded-lg text-white focus:border-yellow-400 focus:outline-none" placeholder="MM/YY" maxlength="5">
                                                </div>
                                                <div>
                                                    <label class="block text-yellow-300 text-sm mb-1">CVV</label>
                                                    <input type="text" id="cardCvv" class="w-full p-3 bg-gray-600/50 border border-yellow-500 rounded-lg text-white focus:border-yellow-400 focus:outline-none" placeholder="123" maxlength="3">
                                                </div>
                                            </div>
                                        </div>
                                    </div>

                                    <!-- Payment Instructions -->
                                    <div id="paymentInstructions" class="bg-gray-700/30 rounded-lg p-4 mb-4 hidden">
                                        <h5 class="text-white font-bold mb-2">📋 Payment Instructions:</h5>
                                        <ol class="text-gray-300 text-sm space-y-1 list-decimal list-inside">
                                            <li>Open your selected payment app</li>
                                            <li>Transfer RM 25.00 to <strong>010-300-6940</strong></li>
                                            <li>Copy the transaction reference ID</li>
                                            <li>Paste it in the field above</li>
                                            <li>Complete your booking</li>
                                        </ol>
                                    </div>

                                    <div class="mt-4 flex items-center justify-between">
                                        <div class="flex items-center space-x-2">
                                            <span class="text-2xl">🔒</span>
                                            <span class="text-green-300 text-sm">Secure Payment Processing</span>
                                        </div>
                                        <div class="text-right">
                                            <p class="text-green-300 font-bold">Total: RM 25.00</p>
                                            <p class="text-gray-400 text-xs">No processing fees</p>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        
                        <div class="md:col-span-2 text-center">
                            <button type="submit" class="bg-gradient-to-r from-green-600 to-green-700 hover:from-green-700 hover:to-green-800 text-white font-bold py-4 px-12 rounded-xl transition-all transform hover:scale-105">
                                💎 Reserve Seat Now
                            </button>
                        </div>
                    </form>
                </div>
            </section>

            <!-- Schedule Section -->
            <section id="scheduleSection" class="max-w-6xl mx-auto hidden">
                <div class="bg-black/40 backdrop-blur-sm rounded-2xl p-8 card-shadow border border-gray-600">
                    <h2 class="text-3xl font-bold text-white mb-8 text-center">🗓️ Game Schedule & Blinds</h2>
                    
                    <div id="scheduleDisplay" class="space-y-6">
                        <!-- Schedule will be loaded here -->
                    </div>
                </div>
            </section>

            <!-- Management Dashboard Section -->
            <section id="managementSection" class="max-w-6xl mx-auto hidden">
                <div id="managementDashboard">
                    <!-- Admin Dashboard -->
                    <div id="adminDashboard" class="hidden">
                        <div class="bg-black/40 backdrop-blur-sm rounded-2xl p-8 card-shadow border border-gray-600">
                            <div class="flex justify-between items-center mb-8">
                                <h2 class="text-3xl font-bold text-white">👑 Admin Management System</h2>
                            </div>
                        
                        <!-- Management Tabs -->
                        <div class="flex space-x-4 mb-8">
                            <button onclick="showAdminTab('schedule')" id="scheduleTabBtn" class="px-4 py-2 bg-blue-600 text-white rounded-lg font-medium transition-all">
                                🗓️ Schedule Management
                            </button>
                            <button onclick="showAdminTab('agents')" id="agentsTabBtn" class="px-4 py-2 bg-gray-600 text-white rounded-lg font-medium transition-all hover:bg-gray-500">
                                👨‍💼 Agent Management
                            </button>
                            <button onclick="showAdminTab('bookings')" id="bookingsTabBtn" class="px-4 py-2 bg-gray-600 text-white rounded-lg font-medium transition-all hover:bg-gray-500">
                                📊 View Bookings
                            </button>
                            <button onclick="showAdminTab('players')" id="playersTabBtn" class="px-4 py-2 bg-gray-600 text-white rounded-lg font-medium transition-all hover:bg-gray-500">
                                👥 Player Registration
                            </button>
                        </div>

                        <!-- Schedule Management Tab -->
                        <div id="scheduleTab" class="space-y-6">
                            <!-- Add New Game -->
                            <div class="bg-gray-700/30 rounded-xl p-6">
                                <h3 class="text-xl font-bold text-white mb-4">➕ Add New Game Session</h3>
                                <form id="addGameForm" class="grid md:grid-cols-4 gap-4">
                                    <div>
                                        <label class="block text-gray-300 font-medium mb-2">Date</label>
                                        <input type="date" id="newGameDate" class="w-full p-3 bg-gray-600/50 border border-gray-500 rounded-lg text-white focus:border-blue-500 focus:outline-none" required>
                                    </div>
                                    <div>
                                        <label class="block text-gray-300 font-medium mb-2">Day Name</label>
                                        <input type="text" id="newGameDay" class="w-full p-3 bg-gray-600/50 border border-gray-500 rounded-lg text-white focus:border-blue-500 focus:outline-none" placeholder="e.g., Monday" required>
                                    </div>
                                    <div>
                                        <label class="block text-gray-300 font-medium mb-2">Start Time</label>
                                        <input type="time" id="newGameTime" class="w-full p-3 bg-gray-600/50 border border-gray-500 rounded-lg text-white focus:border-blue-500 focus:outline-none" required>
                                    </div>
                                    <div class="flex items-end">
                                        <button type="submit" class="w-full bg-gradient-to-r from-green-600 to-green-700 hover:from-green-700 hover:to-green-800 text-white font-bold py-3 rounded-lg transition-all">
                                            Add Game
                                        </button>
                                    </div>
                                </form>
                            </div>
                            
                            <!-- Current Scheduled Games -->
                            <div class="bg-gray-700/30 rounded-xl p-6">
                                <h3 class="text-xl font-bold text-white mb-4">🎮 Current Scheduled Games</h3>
                                <div id="scheduledGamesList" class="space-y-3">
                                    <!-- Games will be loaded here -->
                                </div>
                            </div>
                        </div>

                        <!-- Agent Management Tab -->
                        <div id="agentsTab" class="space-y-6 hidden">
                            <!-- Agent Registration -->
                            <div class="bg-gray-700/30 rounded-xl p-6">
                                <h3 class="text-xl font-bold text-white mb-4">📝 Register New Agent ID</h3>
                                <form id="registerAgentForm" class="grid md:grid-cols-4 gap-4">
                                    <div>
                                        <label class="block text-gray-300 font-medium mb-2">Agent Full Name</label>
                                        <input type="text" id="registerAgentName" class="w-full p-3 bg-gray-600/50 border border-gray-500 rounded-lg text-white focus:border-green-500 focus:outline-none" placeholder="Full Name" required>
                                    </div>
                                    <div>
                                        <label class="block text-gray-300 font-medium mb-2">Phone Number</label>
                                        <input type="tel" id="registerAgentPhone" class="w-full p-3 bg-gray-600/50 border border-gray-500 rounded-lg text-white focus:border-green-500 focus:outline-none" placeholder="+60 12-345 6789" required>
                                    </div>
                                    <div>
                                        <label class="block text-gray-300 font-medium mb-2">Staff ID (Optional)</label>
                                        <input type="text" id="registerAgentStaffId" class="w-full p-3 bg-gray-600/50 border border-gray-500 rounded-lg text-white focus:border-green-500 focus:outline-none" placeholder="880xxxxx">
                                    </div>
                                    <div class="flex items-end">
                                        <button type="submit" class="w-full bg-gradient-to-r from-green-600 to-green-700 hover:from-green-700 hover:to-green-800 text-white font-bold py-3 rounded-lg transition-all">
                                            Register Agent
                                        </button>
                                    </div>
                                </form>
                            </div>

                            <!-- Deploy New Agent -->
                            <div class="bg-gray-700/30 rounded-xl p-6">
                                <h3 class="text-xl font-bold text-white mb-4">👤 Deploy Registered Agent</h3>
                                <form id="deployAgentForm" class="grid md:grid-cols-3 gap-4">
                                    <div>
                                        <label class="block text-gray-300 font-medium mb-2">Select Registered Agent</label>
                                        <select id="selectRegisteredAgent" class="w-full p-3 bg-gray-600/50 border border-gray-500 rounded-lg text-white focus:border-green-500 focus:outline-none" required>
                                            <option value="">Select Agent to Deploy</option>
                                        </select>
                                    </div>
                                    <div>
                                        <label class="block text-gray-300 font-medium mb-2">Agent Login ID</label>
                                        <input type="text" id="newAgentId" class="w-full p-3 bg-gray-600/50 border border-gray-500 rounded-lg text-white focus:border-green-500 focus:outline-none" placeholder="agent5, agent6, etc." required>
                                    </div>
                                    <div class="flex items-end">
                                        <button type="submit" class="w-full bg-gradient-to-r from-blue-600 to-blue-700 hover:from-blue-700 hover:to-blue-800 text-white font-bold py-3 rounded-lg transition-all">
                                            Deploy Agent
                                        </button>
                                    </div>
                                </form>
                            </div>

                            <!-- Active Agents -->
                            <div class="bg-gray-700/30 rounded-xl p-6">
                                <h3 class="text-xl font-bold text-white mb-4">👥 Active Agents</h3>
                                <div id="activeAgentsList" class="space-y-3">
                                    <!-- Agents will be loaded here -->
                                </div>
                            </div>
                        </div>

                        <!-- Bookings Management Tab -->
                        <div id="bookingsTab" class="space-y-6 hidden">
                            <div class="bg-gray-700/30 rounded-xl p-6">
                                <h3 class="text-xl font-bold text-white mb-4">📋 Recent Bookings</h3>
                                <div id="recentBookingsList" class="space-y-3">
                                    <!-- Bookings will be loaded here -->
                                </div>
                            </div>
                        </div>

                        <!-- Player Registration Tab -->
                        <div id="playersTab" class="space-y-6 hidden">
                            <!-- New Player Registration -->
                            <div class="bg-gray-700/30 rounded-xl p-6">
                                <h3 class="text-xl font-bold text-white mb-4">👤 New Player Registration</h3>
                                <form id="playerRegistrationForm" class="grid md:grid-cols-4 gap-4">
                                    <div>
                                        <label class="block text-gray-300 font-medium mb-2">Real Name</label>
                                        <input type="text" id="playerRealName" class="w-full p-3 bg-gray-600/50 border border-gray-500 rounded-lg text-white focus:border-green-500 focus:outline-none" placeholder="Full Real Name" required>
                                    </div>
                                    <div>
                                        <label class="block text-gray-300 font-medium mb-2">Phone Number</label>
                                        <input type="tel" id="playerPhoneNumber" class="w-full p-3 bg-gray-600/50 border border-gray-500 rounded-lg text-white focus:border-green-500 focus:outline-none" placeholder="+60 12-345 6789" required>
                                    </div>
                                    <div>
                                        <label class="block text-gray-300 font-medium mb-2">Staff ID (Optional)</label>
                                        <input type="text" id="playerStaffId" class="w-full p-3 bg-gray-600/50 border border-gray-500 rounded-lg text-white focus:border-green-500 focus:outline-none" placeholder="880xxxxx">
                                    </div>
                                    <div class="flex items-end">
                                        <button type="submit" class="w-full bg-gradient-to-r from-green-600 to-green-700 hover:from-green-700 hover:to-green-800 text-white font-bold py-3 rounded-lg transition-all">
                                            Register Player
                                        </button>
                                    </div>
                                </form>
                            </div>

                            <!-- Registered Players List -->
                            <div class="bg-gray-700/30 rounded-xl p-6">
                                <h3 class="text-xl font-bold text-white mb-4">👥 Registered Players</h3>
                                <div id="registeredPlayersList" class="space-y-3">
                                    <!-- Players will be loaded here -->
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Agent Dashboard -->
                    <div id="agentDashboard" class="hidden">
                        <div class="bg-black/40 backdrop-blur-sm rounded-2xl p-8 card-shadow border border-gray-600">
                            <div class="flex justify-between items-center mb-8">
                                <h2 class="text-3xl font-bold text-white">👨‍💼 Agent Dashboard</h2>
                            </div>
                            
                            <!-- Agent Dashboard Tabs -->
                            <div class="flex space-x-4 mb-8">
                                <button onclick="showAgentTab('sessions')" id="agentSessionsTabBtn" class="px-4 py-2 bg-blue-600 text-white rounded-lg font-medium transition-all">
                                    📊 Session Management
                                </button>
                                <button onclick="showAgentTab('booking')" id="agentBookingTabBtn" class="px-4 py-2 bg-gray-600 text-white rounded-lg font-medium transition-all hover:bg-gray-500">
                                    💺 Book My Seat
                                </button>
                                <button onclick="showAgentTab('history')" id="agentHistoryTabBtn" class="px-4 py-2 bg-gray-600 text-white rounded-lg font-medium transition-all hover:bg-gray-500">
                                    📋 My Bookings
                                </button>
                            </div>
                            
                            <!-- Sessions Tab -->
                            <div id="agentSessionsTab" class="space-y-6">
                                <!-- Agent Stats -->
                                <div class="grid md:grid-cols-4 gap-6 mb-8">
                                    <div class="bg-gradient-to-r from-green-600/20 to-green-800/20 rounded-xl p-6 border border-green-500/30">
                                        <div class="text-center">
                                            <p class="text-3xl font-bold text-white" id="agentTotalRakeBack">$0.00</p>
                                            <p class="text-green-300">Total Commission</p>
                                        </div>
                                    </div>
                                    <div class="bg-gradient-to-r from-blue-600/20 to-blue-800/20 rounded-xl p-6 border border-blue-500/30">
                                        <div class="text-center">
                                            <p class="text-3xl font-bold text-white" id="agentTotalHours">0h</p>
                                            <p class="text-blue-300">Total Hours</p>
                                        </div>
                                    </div>
                                    <div class="bg-gradient-to-r from-purple-600/20 to-purple-800/20 rounded-xl p-6 border border-purple-500/30">
                                        <div class="text-center">
                                            <p class="text-3xl font-bold text-white" id="agentActiveDownlines">0</p>
                                            <p class="text-purple-300">Active Downlines</p>
                                        </div>
                                    </div>
                                    <div class="bg-gradient-to-r from-yellow-600/20 to-yellow-800/20 rounded-xl p-6 border border-yellow-500/30">
                                        <div class="text-center">
                                            <p class="text-3xl font-bold text-white" id="agentTotalSessions">0</p>
                                            <p class="text-yellow-300">Total Sessions</p>
                                        </div>
                                    </div>
                                </div>
                                
                                <!-- Downline Session Entry Form -->
                                <div class="bg-gray-700/30 rounded-xl p-6 mb-8">
                                    <h4 class="text-xl font-bold text-white mb-4">📊 Record Downline Session</h4>
                                    <form id="downlineSessionForm" class="grid md:grid-cols-2 gap-4">
                                        <div>
                                            <label class="block text-gray-300 font-medium mb-2">Player Name</label>
                                            <input type="text" id="sessionPlayerName" class="w-full p-3 bg-gray-600/50 border border-gray-500 rounded-lg text-white focus:border-green-500 focus:outline-none" placeholder="Player name" required>
                                        </div>
                                        <div>
                                            <label class="block text-gray-300 font-medium mb-2">Game Session</label>
                                            <select id="sessionGameSession" class="w-full p-3 bg-gray-600/50 border border-gray-500 rounded-lg text-white focus:border-green-500 focus:outline-none" required>
                                                <option value="">Select Game Session</option>
                                            </select>
                                        </div>
                                        <div>
                                            <label class="block text-gray-300 font-medium mb-2">Start Playing Time</label>
                                            <input type="time" id="sessionStartTime" class="w-full p-3 bg-gray-600/50 border border-gray-500 rounded-lg text-white focus:border-green-500 focus:outline-none" required>
                                        </div>
                                        <div>
                                            <label class="block text-gray-300 font-medium mb-2">End Playing Time</label>
                                            <input type="time" id="sessionEndTime" class="w-full p-3 bg-gray-600/50 border border-gray-500 rounded-lg text-white focus:border-green-500 focus:outline-none" required>
                                        </div>
                                        <div>
                                            <label class="block text-gray-300 font-medium mb-2">Hours Played</label>
                                            <input type="number" id="sessionHours" class="w-full p-3 bg-gray-600/50 border border-gray-500 rounded-lg text-white focus:border-green-500 focus:outline-none" placeholder="0.0" step="0.1" readonly>
                                        </div>
                                        <div>
                                            <label class="block text-gray-300 font-medium mb-2">Rake Back from Player ($)</label>
                                            <input type="number" id="sessionRakeBack" class="w-full p-3 bg-gray-600/50 border border-gray-500 rounded-lg text-white focus:border-green-500 focus:outline-none" placeholder="0.00" step="0.01" required>
                                        </div>
                                        <div>
                                            <label class="block text-gray-300 font-medium mb-2">Commission to Agent ($)</label>
                                            <input type="number" id="sessionCommission" class="w-full p-3 bg-gray-600/50 border border-gray-500 rounded-lg text-white focus:border-green-500 focus:outline-none" placeholder="0.00" step="0.01" required>
                                        </div>
                                        <div>
                                            <label class="block text-gray-300 font-medium mb-2">Player Result</label>
                                            <select id="sessionResult" class="w-full p-3 bg-gray-600/50 border border-gray-500 rounded-lg text-white focus:border-green-500 focus:outline-none" required>
                                                <option value="">Select Result</option>
                                                <option value="win">🟢 Win</option>
                                                <option value="lose">🔴 Lose</option>
                                                <option value="breakeven">🟡 Break Even</option>
                                            </select>
                                        </div>
                                        <div>
                                            <label class="block text-gray-300 font-medium mb-2">Win/Loss Amount ($)</label>
                                            <input type="number" id="sessionWinLoss" class="w-full p-3 bg-gray-600/50 border border-gray-500 rounded-lg text-white focus:border-green-500 focus:outline-none" placeholder="0.00" step="0.01">
                                            <p class="text-gray-400 text-xs mt-1">Positive for wins, negative for losses</p>
                                        </div>
                                        <div>
                                            <label class="block text-gray-300 font-medium mb-2">Notes (Optional)</label>
                                            <input type="text" id="sessionNotes" class="w-full p-3 bg-gray-600/50 border border-gray-500 rounded-lg text-white focus:border-green-500 focus:outline-none" placeholder="Additional notes">
                                        </div>
                                        <div class="md:col-span-2">
                                            <button type="submit" class="w-full bg-gradient-to-r from-green-600 to-green-700 hover:from-green-700 hover:to-green-800 text-white font-bold py-3 rounded-lg transition-all">
                                                📊 Record Session
                                            </button>
                                        </div>
                                    </form>
                                </div>
                                
                                <!-- Downline Activity -->
                                <div class="bg-gray-700/30 rounded-xl p-6 mb-6">
                                    <h4 class="text-xl font-bold text-white mb-4">👥 Downline Activity</h4>
                                    <div id="agentDownlineActivity" class="space-y-3">
                                        <p class="text-gray-400 text-center py-4">No downline activity recorded yet</p>
                                    </div>
                                </div>
                                
                                <!-- Recent Sessions -->
                                <div class="bg-gray-700/30 rounded-xl p-6">
                                    <h4 class="text-xl font-bold text-white mb-4">📋 Recent Sessions</h4>
                                    <div id="agentRecentSessions" class="space-y-3">
                                        <p class="text-gray-400 text-center py-4">No recent sessions</p>
                                    </div>
                                </div>
                            </div>
                            
                            <!-- Agent Booking Tab -->
                            <div id="agentBookingTab" class="space-y-6 hidden">
                                <div class="bg-gray-700/30 rounded-xl p-6">
                                    <h4 class="text-xl font-bold text-white mb-4">💺 Book Your Seat</h4>
                                    <p class="text-gray-300 mb-4">As an agent, you can book seats for yourself to join games. Switch to the main booking section to make your reservation.</p>
                                    <button onclick="showSection('booking')" class="bg-gradient-to-r from-blue-600 to-blue-700 hover:from-blue-700 hover:to-blue-800 text-white font-bold py-3 px-6 rounded-lg transition-all">
                                        🎮 Go to Booking Section
                                    </button>
                                </div>
                            </div>
                            
                            <!-- Agent Booking History Tab -->
                            <div id="agentHistoryTab" class="space-y-6 hidden">
                                <div class="bg-gray-700/30 rounded-xl p-6">
                                    <h4 class="text-xl font-bold text-white mb-4">📋 My Booking History</h4>
                                    <div id="agentBookingHistory" class="space-y-3">
                                        <p class="text-gray-400 text-center py-4">No bookings yet</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Member Dashboard -->
                    <div id="memberDashboard" class="hidden">
                        <div class="bg-black/40 backdrop-blur-sm rounded-2xl p-8 card-shadow border border-gray-600">
                            <div class="flex justify-between items-center mb-8">
                                <h2 class="text-3xl font-bold text-white">👤 Member Dashboard</h2>
                            </div>
                            
                            <!-- Member Stats -->
                            <div class="grid md:grid-cols-3 gap-6 mb-8">
                                <div class="bg-gradient-to-r from-blue-600/20 to-blue-800/20 rounded-xl p-6 border border-blue-500/30">
                                    <div class="text-center">
                                        <p class="text-3xl font-bold text-white" id="memberTotalBookings">0</p>
                                        <p class="text-blue-300">Total Bookings</p>
                                    </div>
                                </div>
                                <div class="bg-gradient-to-r from-green-600/20 to-green-800/20 rounded-xl p-6 border border-green-500/30">
                                    <div class="text-center">
                                        <p class="text-3xl font-bold text-white" id="memberTotalHours">0h</p>
                                        <p class="text-green-300">Hours Played</p>
                                    </div>
                                </div>
                                <div class="bg-gradient-to-r from-purple-600/20 to-purple-800/20 rounded-xl p-6 border border-purple-500/30">
                                    <div class="text-center">
                                        <p class="text-3xl font-bold text-white" id="memberLastSession">Never</p>
                                        <p class="text-purple-300">Last Session</p>
                                    </div>
                                </div>
                            </div>
                            
                            <!-- Member Booking History -->
                            <div class="bg-gray-700/30 rounded-xl p-6">
                                <h4 class="text-xl font-bold text-white mb-4">📋 Your Booking History</h4>
                                <div id="memberBookingHistory" class="space-y-3">
                                    <p class="text-gray-400 text-center py-4">No bookings yet</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>


        </div>

        <!-- Unified Login Modal -->
        <div id="loginModal" class="fixed inset-0 bg-black/70 backdrop-blur-sm hidden items-center justify-center z-50">
            <div class="bg-black/80 rounded-2xl p-8 max-w-md mx-4 card-shadow border border-gray-600">
                <div class="text-center mb-6">
                    <div class="text-4xl mb-2">🔑</div>
                    <h3 class="text-2xl font-bold text-white mb-2">Login to 10K Clubhouse</h3>
                    <p class="text-gray-300 text-sm">Admin, Agent, or Member Access</p>
                </div>
                
                <!-- Login Type Selection -->
                <div class="mb-6">
                    <div class="grid grid-cols-3 gap-2">
                        <button onclick="selectLoginType('admin')" id="adminTypeBtn" class="login-type-btn bg-red-600/30 border-2 border-red-500 p-3 rounded-lg text-center transition-all">
                            <div class="text-2xl mb-1">👑</div>
                            <div class="text-xs text-red-300 font-medium">Admin</div>
                        </button>
                        <button onclick="selectLoginType('agent')" id="agentTypeBtn" class="login-type-btn bg-gray-600/30 border-2 border-gray-500 p-3 rounded-lg text-center transition-all hover:bg-gray-600/50">
                            <div class="text-2xl mb-1">👨‍💼</div>
                            <div class="text-xs text-gray-300 font-medium">Agent</div>
                        </button>
                        <button onclick="selectLoginType('member')" id="memberTypeBtn" class="login-type-btn bg-gray-600/30 border-2 border-gray-500 p-3 rounded-lg text-center transition-all hover:bg-gray-600/50">
                            <div class="text-2xl mb-1">👤</div>
                            <div class="text-xs text-gray-300 font-medium">Member</div>
                        </button>
                    </div>
                </div>
                
                <!-- Login Form -->
                <form id="unifiedLoginForm" class="space-y-4">
                    <div>
                        <label class="block text-gray-300 font-medium mb-2" id="usernameLabel">Username/ID</label>
                        <input type="text" id="loginUsername" class="w-full p-4 bg-gray-800/70 border border-gray-600 rounded-xl text-white focus:border-purple-500 focus:outline-none" placeholder="Enter your username or ID" required>
                    </div>
                    
                    <div>
                        <label class="block text-gray-300 font-medium mb-2">Password</label>
                        <div class="relative">
                            <input type="password" id="loginPassword" class="w-full p-4 pr-12 bg-gray-800/70 border border-gray-600 rounded-xl text-white focus:border-purple-500 focus:outline-none" placeholder="Enter your password" required>
                            <button type="button" onclick="togglePasswordVisibility('loginPassword', 'loginPasswordToggle')" class="absolute right-3 top-1/2 transform -translate-y-1/2 text-gray-400 hover:text-white transition-colors">
                                <span id="loginPasswordToggle">👁️</span>
                            </button>
                        </div>
                    </div>
                    
                    <!-- Member Registration Link -->
                    <div id="memberRegisterLink" class="hidden text-center">
                        <p class="text-gray-400 text-sm">Don't have an account?</p>
                        <button type="button" onclick="showMemberRegistration()" class="text-purple-400 hover:text-purple-300 text-sm underline">
                            Register as Member
                        </button>
                    </div>
                    
                    <div class="flex space-x-3">
                        <button type="submit" class="flex-1 bg-gradient-to-r from-purple-600 to-purple-700 hover:from-purple-700 hover:to-purple-800 text-white font-bold py-4 rounded-xl transition-all">
                            🔑 Login
                        </button>
                        <button type="button" onclick="closeLoginModal()" class="px-6 bg-gray-600 hover:bg-gray-700 text-white font-bold py-4 rounded-xl transition-all">
                            Cancel
                        </button>
                    </div>
                </form>
            </div>
        </div>
        
        <!-- Member Registration Modal -->
        <div id="memberRegisterModal" class="fixed inset-0 bg-black/70 backdrop-blur-sm hidden items-center justify-center z-50">
            <div class="bg-black/80 rounded-2xl p-8 max-w-md mx-4 card-shadow border border-gray-600">
                <div class="text-center mb-6">
                    <div class="text-4xl mb-2">👤</div>
                    <h3 class="text-2xl font-bold text-white mb-2">Member Registration</h3>
                    <p class="text-gray-300 text-sm">Join 10K Clubhouse Community</p>
                </div>
                
                <form id="memberRegisterForm" class="space-y-4">
                    <div>
                        <label class="block text-gray-300 font-medium mb-2">Full Name</label>
                        <input type="text" id="memberName" class="w-full p-4 bg-gray-800/70 border border-gray-600 rounded-xl text-white focus:border-green-500 focus:outline-none" placeholder="Enter your full name" required>
                    </div>
                    
                    <div>
                        <label class="block text-gray-300 font-medium mb-2">Phone Number</label>
                        <input type="tel" id="memberPhone" class="w-full p-4 bg-gray-800/70 border border-gray-600 rounded-xl text-white focus:border-green-500 focus:outline-none" placeholder="+60 12-345 6789" required>
                    </div>
                    
                    <div>
                        <label class="block text-gray-300 font-medium mb-2">Desired Username</label>
                        <input type="text" id="memberUsername" class="w-full p-4 bg-gray-800/70 border border-gray-600 rounded-xl text-white focus:border-green-500 focus:outline-none" placeholder="Choose a username" required>
                    </div>
                    
                    <div>
                        <label class="block text-gray-300 font-medium mb-2">Password</label>
                        <div class="relative">
                            <input type="password" id="memberPassword" class="w-full p-4 pr-12 bg-gray-800/70 border border-gray-600 rounded-xl text-white focus:border-green-500 focus:outline-none" placeholder="Create a password" required>
                            <button type="button" onclick="togglePasswordVisibility('memberPassword', 'memberPasswordToggle')" class="absolute right-3 top-1/2 transform -translate-y-1/2 text-gray-400 hover:text-white transition-colors">
                                <span id="memberPasswordToggle">👁️</span>
                            </button>
                        </div>
                    </div>
                    
                    <div>
                        <label class="block text-gray-300 font-medium mb-2">Staff ID</label>
                        <input type="text" id="memberStaffId" class="w-full p-4 bg-gray-800/70 border border-gray-600 rounded-xl text-white focus:border-green-500 focus:outline-none" placeholder="88xxxxxx" required>
                    </div>
                    
                    <div class="flex space-x-3">
                        <button type="submit" class="flex-1 bg-gradient-to-r from-green-600 to-green-700 hover:from-green-700 hover:to-green-800 text-white font-bold py-4 rounded-xl transition-all">
                            📝 Register
                        </button>
                        <button type="button" onclick="closeMemberRegisterModal()" class="px-6 bg-gray-600 hover:bg-gray-700 text-white font-bold py-4 rounded-xl transition-all">
                            Cancel
                        </button>
                    </div>
                </form>
            </div>
        </div>

        <!-- Success Modal -->
        <div id="successModal" class="fixed inset-0 bg-black/70 backdrop-blur-sm hidden items-center justify-center z-50">
            <div class="bg-black/80 rounded-2xl p-8 max-w-md mx-4 card-shadow border border-gray-600">
                <div class="text-center">
                    <div class="text-6xl mb-4">🎉</div>
                    <h3 class="text-2xl font-bold text-white mb-4">Seat Reserved!</h3>
                    <p class="text-gray-300 mb-6" id="confirmationMessage"></p>
                    <button onclick="closeModal()" class="bg-gradient-to-r from-blue-600 to-blue-700 hover:from-blue-700 hover:to-blue-800 text-white font-bold py-3 px-8 rounded-xl transition-all">
                        Perfect! 💎
                    </button>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Ensure proper initialization
        document.addEventListener('DOMContentLoaded', function() {
            try {
                console.log('10K Clubhouse initializing...');
                initializeApp();
                console.log('10K Clubhouse loaded successfully!');
            } catch (error) {
                console.error('Error loading 10K Clubhouse:', error);
                showErrorMessage();
            }
        });

        function initializeApp() {
            initializeScheduledGames();
            updateGameSessionDropdown();
            loadScheduleDisplay();
            setupEventListeners();
            checkLoginState();
        }
        
        function checkLoginState() {
            const currentUser = localStorage.getItem('currentUser');
            const currentUserName = localStorage.getItem('currentUserName');
            const currentUserRole = localStorage.getItem('currentUserRole');
            
            if (currentUser && currentUserName && currentUserRole) {
                // User is logged in, restore their session
                window.selectedLoginType = currentUserRole;
                
                let userIcon = '👤';
                if (currentUserRole === 'admin') userIcon = '👑';
                else if (currentUserRole === 'agent') userIcon = '👨‍💼';
                
                loginUser(currentUser, currentUserName, userIcon);
                
                // Show appropriate dashboard if they were in management section
                if (currentUserRole === 'admin') {
                    document.getElementById('adminDashboard').classList.remove('hidden');
                    loadAdminData();
                } else if (currentUserRole === 'agent') {
                    document.getElementById('agentDashboard').classList.remove('hidden');
                    loadAgentData(currentUser);
                    updateRakeBackGameDropdown();
                } else if (currentUserRole === 'member') {
                    document.getElementById('memberDashboard').classList.remove('hidden');
                    loadMemberData(currentUser);
                }
            } else {
                // User is not logged in, ensure form is in logged-out state
                resetBookingFormToLoggedOut();
            }
        }

        function showErrorMessage() {
            document.body.innerHTML = `
                <div class="min-h-screen bg-gray-900 flex items-center justify-center">
                    <div class="text-center text-white">
                        <h1 class="text-4xl font-bold mb-4">🏆 10K Clubhouse</h1>
                        <p class="text-xl mb-4">Loading...</p>
                        <p class="text-gray-400">If this persists, please refresh the page</p>
                    </div>
                </div>
            `;
        }

        function setupEventListeners() {
            // Show/hide payment section and reservation reminder
            const seatSelect = document.getElementById('seatReservation');
            if (seatSelect) {
                seatSelect.addEventListener('change', function() {
                    const paymentSection = document.getElementById('paymentSection');
                    const reservationReminder = document.getElementById('reservationReminder');
                    
                    if (this.value.startsWith('25_')) {
                        paymentSection.classList.remove('hidden');
                        reservationReminder.classList.remove('hidden');
                        // Default to Touch 'n Go
                        selectPaymentMethod('tng');
                    } else {
                        paymentSection.classList.add('hidden');
                        reservationReminder.classList.add('hidden');
                    }
                });
            }

            // Format card inputs
            setupCardFormatting();
            setupFormSubmissions();
        }

        // Payment method selection
        function selectPaymentMethod(method) {
            // Reset all payment method buttons
            const buttons = ['tngBtn', 'grabpayBtn', 'boostBtn', 'cardBtn'];
            buttons.forEach(btnId => {
                const btn = document.getElementById(btnId);
                if (btn) {
                    btn.className = 'payment-method-btn bg-gray-600/30 border-2 border-gray-500 p-3 rounded-lg text-center transition-all hover:bg-gray-600/50';
                }
            });

            // Hide all payment forms
            const forms = ['tngPayment', 'grabpayPayment', 'boostPayment', 'cardPayment'];
            forms.forEach(formId => {
                const form = document.getElementById(formId);
                if (form) form.classList.add('hidden');
            });

            // Show selected method
            if (method === 'tng') {
                document.getElementById('tngBtn').className = 'payment-method-btn bg-blue-600/30 border-2 border-blue-500 p-3 rounded-lg text-center transition-all hover:bg-blue-600/50';
                document.getElementById('tngPayment').classList.remove('hidden');
                document.getElementById('paymentInstructions').classList.remove('hidden');
            } else if (method === 'grabpay') {
                document.getElementById('grabpayBtn').className = 'payment-method-btn bg-green-600/30 border-2 border-green-500 p-3 rounded-lg text-center transition-all hover:bg-green-600/50';
                document.getElementById('grabpayPayment').classList.remove('hidden');
                document.getElementById('paymentInstructions').classList.remove('hidden');
            } else if (method === 'boost') {
                document.getElementById('boostBtn').className = 'payment-method-btn bg-purple-600/30 border-2 border-purple-500 p-3 rounded-lg text-center transition-all hover:bg-purple-600/50';
                document.getElementById('boostPayment').classList.remove('hidden');
                document.getElementById('paymentInstructions').classList.remove('hidden');
            } else if (method === 'card') {
                document.getElementById('cardBtn').className = 'payment-method-btn bg-yellow-600/30 border-2 border-yellow-500 p-3 rounded-lg text-center transition-all hover:bg-yellow-600/50';
                document.getElementById('cardPayment').classList.remove('hidden');
                document.getElementById('paymentInstructions').classList.add('hidden');
            }

            // Store selected payment method
            window.selectedPaymentMethod = method;
        }

        function setupCardFormatting() {
            // Format card number input
            const cardNumber = document.getElementById('cardNumber');
            if (cardNumber) {
                cardNumber.addEventListener('input', function(e) {
                    let value = e.target.value.replace(/\s/g, '').replace(/[^0-9]/gi, '');
                    let formattedValue = value.match(/.{1,4}/g)?.join(' ') || value;
                    if (formattedValue.length > 19) formattedValue = formattedValue.substr(0, 19);
                    e.target.value = formattedValue;
                });
            }

            // Format expiry date input
            const cardExpiry = document.getElementById('cardExpiry');
            if (cardExpiry) {
                cardExpiry.addEventListener('input', function(e) {
                    let value = e.target.value.replace(/\D/g, '');
                    if (value.length >= 2) {
                        value = value.substring(0, 2) + '/' + value.substring(2, 4);
                    }
                    e.target.value = value;
                });
            }

            // Format CVV input
            const cardCvv = document.getElementById('cardCvv');
            if (cardCvv) {
                cardCvv.addEventListener('input', function(e) {
                    e.target.value = e.target.value.replace(/\D/g, '').substring(0, 3);
                });
            }
        }

        function setupFormSubmissions() {
            // Booking form submission
            const bookingForm = document.getElementById('bookingForm');
            if (bookingForm) {
                bookingForm.addEventListener('submit', handleBookingSubmission);
            }

            // Unified login form
            const unifiedLoginForm = document.getElementById('unifiedLoginForm');
            if (unifiedLoginForm) {
                unifiedLoginForm.addEventListener('submit', handleUnifiedLogin);
            }

            // Member registration form
            const memberRegisterForm = document.getElementById('memberRegisterForm');
            if (memberRegisterForm) {
                memberRegisterForm.addEventListener('submit', handleMemberRegistration);
            }

            // Downline session form
            const downlineSessionForm = document.getElementById('downlineSessionForm');
            if (downlineSessionForm) {
                downlineSessionForm.addEventListener('submit', handleDownlineSessionSubmission);
            }

            // Add game form
            const addGameForm = document.getElementById('addGameForm');
            if (addGameForm) {
                addGameForm.addEventListener('submit', handleAddGame);
            }

            // Deploy agent form
            const deployAgentForm = document.getElementById('deployAgentForm');
            if (deployAgentForm) {
                deployAgentForm.addEventListener('submit', handleDeployAgent);
            }

            // Register agent form
            const registerAgentForm = document.getElementById('registerAgentForm');
            if (registerAgentForm) {
                registerAgentForm.addEventListener('submit', handleRegisterAgent);
            }

            // Player registration form
            const playerRegistrationForm = document.getElementById('playerRegistrationForm');
            if (playerRegistrationForm) {
                playerRegistrationForm.addEventListener('submit', handlePlayerRegistration);
            }

            // Player Activity Tracking form
            const playerActivityForm = document.getElementById('playerActivityForm');
            if (playerActivityForm) {
                playerActivityForm.addEventListener('submit', handlePlayerActivity);
            }

            // Change password form
            const changePasswordForm = document.getElementById('changePasswordForm');
            if (changePasswordForm) {
                changePasswordForm.addEventListener('submit', handleChangePassword);
            }

            // Auto-calculate hours played for session form
            const sessionStartTime = document.getElementById('sessionStartTime');
            const sessionEndTime = document.getElementById('sessionEndTime');
            const sessionHours = document.getElementById('sessionHours');
            
            if (sessionStartTime && sessionEndTime && sessionHours) {
                [sessionStartTime, sessionEndTime].forEach(input => {
                    input.addEventListener('change', calculateSessionHours);
                });
            }
        }

        function calculateSessionHours() {
            const startTime = document.getElementById('sessionStartTime').value;
            const endTime = document.getElementById('sessionEndTime').value;
            
            if (startTime && endTime) {
                const start = new Date('2000-01-01 ' + startTime);
                const end = new Date('2000-01-01 ' + endTime);
                
                // Handle next day scenario
                if (end < start) {
                    end.setDate(end.getDate() + 1);
                }
                
                const diffMs = end - start;
                const hours = diffMs / (1000 * 60 * 60);
                
                document.getElementById('sessionHours').value = hours.toFixed(1);
            }
        }

        // Password visibility toggle
        function togglePasswordVisibility(inputId, toggleId) {
            const passwordInput = document.getElementById(inputId);
            const toggleIcon = document.getElementById(toggleId);
            
            if (passwordInput.type === 'password') {
                passwordInput.type = 'text';
                toggleIcon.textContent = '🙈';
            } else {
                passwordInput.type = 'password';
                toggleIcon.textContent = '👁️';
            }
        }

        // Unified Login Handler
        function handleUnifiedLogin(e) {
            e.preventDefault();
            
            const username = document.getElementById('loginUsername').value;
            const password = document.getElementById('loginPassword').value;
            const loginType = window.selectedLoginType || 'admin';
            
            if (loginType === 'admin') {
                handleAdminLogin(username, password);
            } else if (loginType === 'agent') {
                handleAgentLogin(username, password);
            } else if (loginType === 'member') {
                handleMemberLogin(username, password);
            }
        }

        function handleAdminLogin(username, password) {
            // Admin credentials - Fixed login issue
            console.log('Admin login attempt:', username, password); // Debug log
            if ((username === 'admin' || username === 'administrator') && password === 'poker2024admin') {
                loginUser('admin', 'Administrator', '👑');
                showSection('management');
                document.getElementById('adminDashboard').classList.remove('hidden');
                document.getElementById('managementSection').classList.remove('hidden');
                loadAdminData();
                closeLoginModal();
                alert('✅ Admin login successful! Welcome to the management dashboard.');
            } else {
                alert(`❌ Invalid admin credentials!\n\nCorrect credentials:\nUsername: admin\nPassword: poker2024admin`);
            }
        }

        function handleAgentLogin(username, password) {
            // Get deployed agents
            const agents = JSON.parse(localStorage.getItem('deployedAgents') || '[]');
            const agent = agents.find(a => a.id === username && a.password === password && a.active);
            
            if (agent) {
                loginUser(username, agent.name, '👨‍💼');
                showSection('management');
                document.getElementById('agentDashboard').classList.remove('hidden');
                loadAgentData(username);
                updateRakeBackGameDropdown();
                closeLoginModal();
            } else {
                alert('❌ Invalid agent credentials or account inactive!');
            }
        }

        function handleMemberLogin(username, password) {
            // Get registered members
            const members = JSON.parse(localStorage.getItem('registeredMembers') || '[]');
            const member = members.find(m => m.username === username && m.password === password && m.active);
            
            if (member) {
                loginUser(username, member.name, '👤');
                showSection('management');
                document.getElementById('memberDashboard').classList.remove('hidden');
                loadMemberData(username);
                closeLoginModal();
            } else {
                alert('❌ Invalid member credentials or account inactive!');
            }
        }

        function handleMemberRegistration(e) {
            e.preventDefault();
            
            const name = document.getElementById('memberName').value;
            const phone = document.getElementById('memberPhone').value;
            const username = document.getElementById('memberUsername').value;
            const password = document.getElementById('memberPassword').value;
            const staffId = document.getElementById('memberStaffId').value;
            
            if (!staffId) {
                alert('Staff ID is required for member registration!');
                return;
            }
            
            let members = JSON.parse(localStorage.getItem('registeredMembers') || '[]');
            
            // Check if username, phone, or staff ID already exists
            if (members.some(m => m.username === username)) {
                alert('Username already exists! Please choose a different one.');
                return;
            }
            
            if (members.some(m => m.phone === phone)) {
                alert('Phone number already registered!');
                return;
            }
            
            if (members.some(m => m.staffId === staffId)) {
                alert('Staff ID already registered!');
                return;
            }
            
            const newMember = {
                id: Date.now(),
                name: name,
                phone: phone,
                username: username,
                password: password,
                staffId: staffId,
                registered: new Date().toISOString(),
                active: true
            };
            
            members.push(newMember);
            localStorage.setItem('registeredMembers', JSON.stringify(members));
            
            closeMemberRegisterModal();
            alert(`🎉 Registration successful!\nWelcome to 10K Clubhouse, ${name}!\nYou can now login with username: ${username}`);
        }

        function handleDownlineSessionSubmission(e) {
            e.preventDefault();
            
            const currentAgent = localStorage.getItem('currentUser');
            const playerName = document.getElementById('sessionPlayerName').value;
            const gameSession = document.getElementById('sessionGameSession').value;
            const startTime = document.getElementById('sessionStartTime').value;
            const endTime = document.getElementById('sessionEndTime').value;
            const hoursPlayed = parseFloat(document.getElementById('sessionHours').value);
            const rakeBackAmount = parseFloat(document.getElementById('sessionRakeBack').value);
            const commissionAmount = parseFloat(document.getElementById('sessionCommission').value);
            const playerResult = document.getElementById('sessionResult').value;
            const winLossAmount = parseFloat(document.getElementById('sessionWinLoss').value) || 0;
            const notes = document.getElementById('sessionNotes').value;
            
            // Get game date from session
            const scheduledGames = JSON.parse(localStorage.getItem('scheduledGames') || '[]');
            const selectedGame = scheduledGames.find(game => game.displayText === gameSession);
            const gameDate = selectedGame ? selectedGame.date : new Date().toISOString().split('T')[0];
            
            const sessionRecord = {
                id: Date.now(),
                agentId: currentAgent,
                playerName: playerName,
                gameSession: gameSession,
                gameDate: gameDate,
                startTime: startTime,
                endTime: endTime,
                hoursPlayed: hoursPlayed,
                rakeBackAmount: rakeBackAmount,
                commissionAmount: commissionAmount,
                playerResult: playerResult,
                winLossAmount: winLossAmount,
                notes: notes,
                date: new Date().toLocaleDateString(),
                timestamp: new Date().toISOString()
            };
            
            // Save session record
            let sessionRecords = JSON.parse(localStorage.getItem('downlineSessionRecords') || '[]');
            sessionRecords.push(sessionRecord);
            localStorage.setItem('downlineSessionRecords', JSON.stringify(sessionRecords));
            
            // Reset form
            document.getElementById('downlineSessionForm').reset();
            
            // Reload agent data
            loadAgentData(currentAgent);
            
            alert('📊 Downline session recorded successfully!');
        }

        function loginUser(userId, userName, userIcon) {
            // Store current user
            localStorage.setItem('currentUser', userId);
            localStorage.setItem('currentUserName', userName);
            localStorage.setItem('currentUserRole', window.selectedLoginType);
            
            // Update UI
            document.getElementById('loginBtn').classList.add('hidden');
            document.getElementById('userInfo').classList.remove('hidden');
            document.getElementById('userAvatar').textContent = userIcon;
            document.getElementById('userName').textContent = userName;
            
            let roleText = '';
            if (window.selectedLoginType === 'admin') roleText = 'Administrator';
            else if (window.selectedLoginType === 'agent') roleText = 'Agent';
            else if (window.selectedLoginType === 'member') roleText = 'Member';
            
            document.getElementById('userRole').textContent = roleText;
            
            // Enable booking features for members and agents
            if (window.selectedLoginType === 'member') {
                enableMemberBookingFeatures(userName);
            } else if (window.selectedLoginType === 'agent') {
                enableAgentBookingFeatures(userName);
            }
        }
        
        function enableMemberBookingFeatures(memberName) {
            // Auto-fill player name with registered member name
            const playerNameField = document.getElementById('playerName');
            if (playerNameField) {
                playerNameField.value = memberName;
                playerNameField.readOnly = true;
            }
            
            // Enable seat reservation dropdown
            const seatReservation = document.getElementById('seatReservation');
            if (seatReservation) {
                seatReservation.disabled = false;
                seatReservation.innerHTML = `
                    <option value="">No Reservation</option>
                    <option value="none">No seat reservation is required</option>
                    <option value="25_2">Seat 2 - RM 25 💳</option>
                    <option value="25_3">Seat 3 - RM 25 💳</option>
                    <option value="25_4">Seat 4 - RM 25 💳</option>
                    <option value="25_5">Seat 5 - RM 25 💳</option>
                    <option value="25_6">Seat 6 - RM 25 💳</option>
                    <option value="25_7">Seat 7 - RM 25 💳</option>
                    <option value="25_8">Seat 8 - RM 25 💳</option>
                    <option value="25_9">Seat 9 - RM 25 💳</option>
                    <option value="25_10">Seat 10 - RM 25 💳</option>
                `;
            }
        }
        
        function enableAgentBookingFeatures(agentName) {
            // Auto-fill player name with agent name
            const playerNameField = document.getElementById('playerName');
            if (playerNameField) {
                playerNameField.value = agentName;
                playerNameField.readOnly = true;
            }
            
            // Enable seat reservation dropdown for agents
            const seatReservation = document.getElementById('seatReservation');
            if (seatReservation) {
                seatReservation.disabled = false;
                seatReservation.innerHTML = `
                    <option value="">No Reservation</option>
                    <option value="none">No seat reservation is required</option>
                    <option value="25_2">Seat 2 - RM 25 💳</option>
                    <option value="25_3">Seat 3 - RM 25 💳</option>
                    <option value="25_4">Seat 4 - RM 25 💳</option>
                    <option value="25_5">Seat 5 - RM 25 💳</option>
                    <option value="25_6">Seat 6 - RM 25 💳</option>
                    <option value="25_7">Seat 7 - RM 25 💳</option>
                    <option value="25_8">Seat 8 - RM 25 💳</option>
                    <option value="25_9">Seat 9 - RM 25 💳</option>
                    <option value="25_10">Seat 10 - RM 25 💳</option>
                `;
            }
        }

        function logout() {
            // Clear user data
            localStorage.removeItem('currentUser');
            localStorage.removeItem('currentUserName');
            localStorage.removeItem('currentUserRole');
            
            // Update UI
            document.getElementById('loginBtn').classList.remove('hidden');
            document.getElementById('userInfo').classList.add('hidden');
            
            // Hide all dashboards
            document.getElementById('adminDashboard').classList.add('hidden');
            document.getElementById('agentDashboard').classList.add('hidden');
            document.getElementById('memberDashboard').classList.add('hidden');
            document.getElementById('managementSection').classList.add('hidden');
            
            // Reset booking form to logged-out state
            resetBookingFormToLoggedOut();
            
            // Show booking section
            showSection('booking');
        }
        
        function resetBookingFormToLoggedOut() {
            // Clear and disable player name field
            const playerNameField = document.getElementById('playerName');
            if (playerNameField) {
                playerNameField.value = '';
                playerNameField.readOnly = true;
                playerNameField.placeholder = 'Enter your name';
            }
            
            // Disable seat reservation dropdown
            const seatReservation = document.getElementById('seatReservation');
            if (seatReservation) {
                seatReservation.disabled = true;
                seatReservation.innerHTML = '<option value="">🔒 Login required to reserve seats</option>';
            }
            
            // Hide payment section
            const paymentSection = document.getElementById('paymentSection');
            if (paymentSection) {
                paymentSection.classList.add('hidden');
            }
        }

        function updateRakeBackGameDropdown() {
            const scheduledGames = JSON.parse(localStorage.getItem('scheduledGames') || '[]');
            const dropdown = document.getElementById('sessionGameSession');
            
            if (dropdown) {
                dropdown.innerHTML = '<option value="">Select Game Session</option>';
                
                scheduledGames.forEach(game => {
                    const option = document.createElement('option');
                    option.value = game.displayText;
                    option.textContent = game.displayText;
                    dropdown.appendChild(option);
                });
            }
        }

        // Navigation
        function showSection(section) {
            // Hide all sections
            const sections = ['bookingSection', 'scheduleSection', 'managementSection'];
            sections.forEach(s => {
                const element = document.getElementById(s);
                if (element) element.classList.add('hidden');
            });
            
            // Reset button styles
            const buttons = ['bookingBtn', 'scheduleBtn'];
            buttons.forEach(b => {
                const element = document.getElementById(b);
                if (element) {
                    element.className = 'px-6 py-3 rounded-full text-gray-300 hover:bg-gray-700 font-medium mx-2 transition-all';
                }
            });
            
            // Show selected section and highlight button
            if (section === 'booking') {
                document.getElementById('bookingSection').classList.remove('hidden');
                document.getElementById('bookingBtn').className = 'px-6 py-3 rounded-full bg-blue-600 text-white font-medium mx-2 transition-all';
            } else if (section === 'schedule') {
                document.getElementById('scheduleSection').classList.remove('hidden');
                document.getElementById('scheduleBtn').className = 'px-6 py-3 rounded-full bg-blue-600 text-white font-medium mx-2 transition-all';
                loadScheduleDisplay();
            } else if (section === 'management') {
                document.getElementById('managementSection').classList.remove('hidden');
            }
        }

        // Login Modal Functions
        function showLoginModal() {
            document.getElementById('loginModal').classList.remove('hidden');
            document.getElementById('loginModal').classList.add('flex');
            // Default to admin login type
            selectLoginType('admin');
        }

        function closeLoginModal() {
            document.getElementById('loginModal').classList.add('hidden');
            document.getElementById('loginModal').classList.remove('flex');
            document.getElementById('unifiedLoginForm').reset();
        }

        function selectLoginType(type) {
            // Reset all login type buttons
            const buttons = ['adminTypeBtn', 'agentTypeBtn', 'memberTypeBtn'];
            buttons.forEach(btnId => {
                const btn = document.getElementById(btnId);
                if (btn) {
                    btn.className = 'login-type-btn bg-gray-600/30 border-2 border-gray-500 p-3 rounded-lg text-center transition-all hover:bg-gray-600/50';
                }
            });

            // Update labels and placeholders based on type
            const usernameLabel = document.getElementById('usernameLabel');
            const usernameInput = document.getElementById('loginUsername');
            const memberRegisterLink = document.getElementById('memberRegisterLink');

            if (type === 'admin') {
                document.getElementById('adminTypeBtn').className = 'login-type-btn bg-red-600/30 border-2 border-red-500 p-3 rounded-lg text-center transition-all';
                usernameLabel.textContent = 'Admin Username';
                usernameInput.placeholder = 'Enter admin username';
                memberRegisterLink.classList.add('hidden');
            } else if (type === 'agent') {
                document.getElementById('agentTypeBtn').className = 'login-type-btn bg-blue-600/30 border-2 border-blue-500 p-3 rounded-lg text-center transition-all';
                usernameLabel.textContent = 'Agent ID';
                usernameInput.placeholder = 'Enter agent ID';
                memberRegisterLink.classList.add('hidden');
            } else if (type === 'member') {
                document.getElementById('memberTypeBtn').className = 'login-type-btn bg-green-600/30 border-2 border-green-500 p-3 rounded-lg text-center transition-all';
                usernameLabel.textContent = 'Username';
                usernameInput.placeholder = 'Enter your username';
                memberRegisterLink.classList.remove('hidden');
            }

            // Store selected login type
            window.selectedLoginType = type;
        }

        function showMemberRegistration() {
            closeLoginModal();
            document.getElementById('memberRegisterModal').classList.remove('hidden');
            document.getElementById('memberRegisterModal').classList.add('flex');
        }

        function closeMemberRegisterModal() {
            document.getElementById('memberRegisterModal').classList.add('hidden');
            document.getElementById('memberRegisterModal').classList.remove('flex');
            document.getElementById('memberRegisterForm').reset();
        }

        function handleBookingSubmission(e) {
            e.preventDefault();
            
            // Check if user is logged in as member or agent for seat reservations
            const currentUser = localStorage.getItem('currentUser');
            const currentUserRole = localStorage.getItem('currentUserRole');
            const seatReservation = document.getElementById('seatReservation').value;
            
            if (seatReservation.startsWith('25_') && (!currentUser || (currentUserRole !== 'member' && currentUserRole !== 'agent'))) {
                alert('🔒 Please login as a member or agent to reserve seats!');
                showLoginModal();
                return;
            }
            
            const playerName = document.getElementById('playerName').value;
            const gameSession = document.getElementById('gameSession').value;
            const gameTime = document.getElementById('gameTime').value;
            const agent = document.getElementById('referringAgent').value;
            const foodOrder = document.getElementById('foodOrder').value;
            
            // Get game session details
            const scheduledGames = JSON.parse(localStorage.getItem('scheduledGames') || '[]');
            const selectedGame = scheduledGames.find(game => `${game.date}_${game.time}` === gameSession);
            
            if (!selectedGame) {
                alert('Please select a valid game session');
                return;
            }

            // Validate payment if seat reservation is selected
            if (seatReservation.startsWith('25_')) {
                const paymentMethod = window.selectedPaymentMethod || 'tng';
                
                if (paymentMethod === 'tng') {
                    const tngPhone = document.getElementById('tngPhone').value;
                    const tngRef = document.getElementById('tngRef').value;
                    
                    if (!tngPhone || !tngRef) {
                        alert('📱 Please complete Touch \'n Go payment details');
                        return;
                    }
                    
                    if (tngPhone.length < 10) {
                        alert('📱 Please enter a valid phone number');
                        return;
                    }
                    
                } else if (paymentMethod === 'grabpay') {
                    const grabPhone = document.getElementById('grabPhone').value;
                    const grabRef = document.getElementById('grabRef').value;
                    
                    if (!grabPhone || !grabRef) {
                        alert('🚗 Please complete GrabPay payment details');
                        return;
                    }
                    
                } else if (paymentMethod === 'boost') {
                    const boostPhone = document.getElementById('boostPhone').value;
                    const boostRef = document.getElementById('boostRef').value;
                    
                    if (!boostPhone || !boostRef) {
                        alert('🚀 Please complete Boost payment details');
                        return;
                    }
                    
                } else if (paymentMethod === 'card') {
                    const cardNumber = document.getElementById('cardNumber').value;
                    const cardName = document.getElementById('cardName').value;
                    const cardExpiry = document.getElementById('cardExpiry').value;
                    const cardCvv = document.getElementById('cardCvv').value;

                    if (!cardNumber || !cardName || !cardExpiry || !cardCvv) {
                        alert('💳 Please complete all card details for seat reservation');
                        return;
                    }

                    if (cardNumber.replace(/\s/g, '').length < 16) {
                        alert('💳 Please enter a valid card number');
                        return;
                    }

                    if (cardExpiry.length < 5) {
                        alert('💳 Please enter a valid expiry date (MM/YY)');
                        return;
                    }

                    if (cardCvv.length < 3) {
                        alert('💳 Please enter a valid CVV');
                        return;
                    }
                }

                // Simulate payment processing
                showPaymentProcessing(() => completeBooking());
            } else {
                completeBooking();
            }

            function completeBooking() {
                // Store booking data
                const seatNumber = seatReservation ? seatReservation.split('_')[1] : null;
                const paymentMethod = window.selectedPaymentMethod || 'tng';
                
                // Get payment details based on method
                let paymentDetails = {};
                if (seatReservation.startsWith('25_')) {
                    if (paymentMethod === 'tng') {
                        paymentDetails = {
                            method: 'Touch \'n Go',
                            phone: document.getElementById('tngPhone').value,
                            reference: document.getElementById('tngRef').value
                        };
                    } else if (paymentMethod === 'grabpay') {
                        paymentDetails = {
                            method: 'GrabPay',
                            phone: document.getElementById('grabPhone').value,
                            reference: document.getElementById('grabRef').value
                        };
                    } else if (paymentMethod === 'boost') {
                        paymentDetails = {
                            method: 'Boost',
                            phone: document.getElementById('boostPhone').value,
                            reference: document.getElementById('boostRef').value
                        };
                    } else if (paymentMethod === 'card') {
                        paymentDetails = {
                            method: 'Credit Card',
                            cardLast4: document.getElementById('cardNumber').value.slice(-4),
                            cardName: document.getElementById('cardName').value
                        };
                    }
                }
                
                const booking = {
                    id: Date.now(),
                    playerName,
                    gameSession: selectedGame.displayText,
                    gameDate: selectedGame.date,
                    gameStartTime: selectedGame.time,
                    arrivalTime: gameTime,
                    seatReservation,
                    seatNumber,
                    agent,
                    foodOrder: foodOrder || null,
                    paymentStatus: seatReservation.startsWith('25_') ? 'Paid' : 'No Payment',
                    paymentMethod: paymentMethod,
                    paymentDetails: paymentDetails,
                    timestamp: new Date().toISOString()
                };
                
                // Save to localStorage
                let bookings = JSON.parse(localStorage.getItem('pokerBookings') || '[]');
                bookings.push(booking);
                localStorage.setItem('pokerBookings', JSON.stringify(bookings));
                
                // Show confirmation
                showBookingConfirmation(booking, selectedGame);
                
                // Reset form
                document.getElementById('bookingForm').reset();
                document.getElementById('paymentSection').classList.add('hidden');
            }
        }

        function showPaymentProcessing(callback) {
            const processingModal = document.createElement('div');
            processingModal.className = 'fixed inset-0 bg-black/70 backdrop-blur-sm flex items-center justify-center z-50';
            processingModal.innerHTML = `
                <div class="bg-black/80 rounded-2xl p-8 max-w-md mx-4 text-center border border-gray-600">
                    <div class="animate-spin text-6xl mb-4">💳</div>
                    <h3 class="text-2xl font-bold text-white mb-2">Processing Payment...</h3>
                    <p class="text-gray-300">Please wait while we process your RM 25.00 payment</p>
                </div>
            `;
            document.body.appendChild(processingModal);

            // Simulate processing delay
            setTimeout(() => {
                document.body.removeChild(processingModal);
                callback();
            }, 2000);
        }

        function showBookingConfirmation(booking, selectedGame) {
            const arrivalOptions = {
                'same': 'Same as game start time',
                '15min': '15 minutes after start',
                '30min': '30 minutes after start',
                '1hour': '1 hour after start'
            };
            
            let paymentInfo = '';
            if (booking.seatReservation && booking.seatReservation.startsWith('25_')) {
                paymentInfo = `💺 Seat ${booking.seatNumber} Reserved: RM 25 ✅<br>`;
                paymentInfo += `🎰 Fee will be returned as chips upon arrival!<br>`;
                if (booking.paymentDetails.method) {
                    paymentInfo += `💳 ${booking.paymentDetails.method} Payment Confirmed<br>`;
                    if (booking.paymentDetails.reference) {
                        paymentInfo += `📋 Ref: ${booking.paymentDetails.reference}<br>`;
                    }
                }
            }
            
            let foodInfo = '';
            if (booking.foodOrder) {
                foodInfo = `🍽️ Food Order: ${booking.foodOrder}<br>📅 Will be prepared around your arrival time<br>`;
            }
            
            document.getElementById('confirmationMessage').innerHTML = `
                <strong>${booking.playerName}</strong><br>
                🗓️ ${selectedGame.displayText}<br>
                ⏰ Arrival: ${arrivalOptions[booking.arrivalTime]}<br>
                ${paymentInfo}
                ${foodInfo}
                💎 Your booking is confirmed!
            `;
            
            document.getElementById('successModal').classList.remove('hidden');
            document.getElementById('successModal').classList.add('flex');
        }

        function handleAgentLogin(e) {
            e.preventDefault();
            
            const agentId = document.getElementById('agentId').value;
            const password = document.getElementById('agentPassword').value;
            
            // Simple authentication (in real app, this would be server-side)
            const validAgents = {
                'agent1': { name: 'Mike Chen', password: 'poker123' },
                'agent2': { name: 'Sarah Johnson', password: 'poker123' },
                'agent3': { name: 'David Rodriguez', password: 'poker123' },
                'agent4': { name: 'Lisa Wang', password: 'poker123' }
            };
            
            if (validAgents[agentId] && validAgents[agentId].password === password) {
                document.getElementById('agentLogin').classList.add('hidden');
                document.getElementById('agentDashboard').classList.remove('hidden');
                document.getElementById('agentName').textContent = validAgents[agentId].name;
                
                // Store current agent
                localStorage.setItem('currentAgent', agentId);
                
                // Load agent data
                loadAgentData(agentId);
            } else {
                alert('Invalid credentials. Please try again.');
            }
        }

        function handleRewardSubmission(e) {
            e.preventDefault();
            
            const currentAgent = localStorage.getItem('currentAgent');
            const playerName = document.getElementById('rewardPlayerName').value;
            const amount = parseFloat(document.getElementById('rewardAmount').value);
            
            const reward = {
                id: Date.now(),
                agent: currentAgent,
                playerName,
                amount,
                date: new Date().toLocaleDateString(),
                timestamp: new Date().toISOString()
            };
            
            // Save reward
            let rewards = JSON.parse(localStorage.getItem('agentRewards') || '[]');
            rewards.push(reward);
            localStorage.setItem('agentRewards', JSON.stringify(rewards));
            
            // Reset form
            document.getElementById('rewardForm').reset();
            
            // Reload agent data
            loadAgentData(currentAgent);
            
            alert('Reward added successfully! 💰');
        }

        function handleAdminLogin(e) {
            e.preventDefault();
            
            const username = document.getElementById('adminUsername').value;
            const password = document.getElementById('adminPassword').value;
            
            // Admin credentials (in real app, this would be server-side)
            if (username === 'admin' && password === 'poker2024admin') {
                document.getElementById('adminLogin').classList.add('hidden');
                document.getElementById('adminDashboard').classList.remove('hidden');
                loadAdminData();
            } else {
                alert('❌ Invalid admin credentials!');
            }
        }

        function handleAddGame(e) {
            e.preventDefault();
            
            const dateInput = document.getElementById('newGameDate').value;
            const dayInput = document.getElementById('newGameDay').value;
            const timeInput = document.getElementById('newGameTime').value;
            
            if (!dateInput || !dayInput || !timeInput) return;
            
            // Format time for display
            const timeObj = new Date('2000-01-01 ' + timeInput);
            const displayTime = timeObj.toLocaleTimeString('en-US', { 
                hour: 'numeric', 
                minute: '2-digit',
                hour12: true 
            });
            
            const dateObj = new Date(dateInput);
            const months = ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec'];
            const displayText = `${dayInput}, ${months[dateObj.getMonth()]} ${dateObj.getDate()}, ${dateObj.getFullYear()} at ${displayTime}`;
            
            const newGame = {
                id: Date.now(),
                date: dateInput,
                day: dayInput,
                time: timeInput,
                displayText: displayText
            };
            
            let scheduledGames = JSON.parse(localStorage.getItem('scheduledGames') || '[]');
            
            // Check if game already exists
            if (scheduledGames.some(g => g.date === dateInput && g.time === timeInput)) {
                alert('A game is already scheduled for this date and time!');
                return;
            }
            
            scheduledGames.push(newGame);
            scheduledGames.sort((a, b) => new Date(a.date + ' ' + a.time) - new Date(b.date + ' ' + b.time));
            
            localStorage.setItem('scheduledGames', JSON.stringify(scheduledGames));
            
            document.getElementById('addGameForm').reset();
            loadScheduledGames();
            updateGameSessionDropdown();
            loadScheduleDisplay();
            updateActivityGameDropdown();
            
            alert('Game session added successfully! 🎮');
        }

        function calculateHours() {
            const arrivalTime = document.getElementById('activityArrival').value;
            const leaveTime = document.getElementById('activityLeave').value;
            
            if (arrivalTime && leaveTime) {
                const arrival = new Date('2000-01-01 ' + arrivalTime);
                const leave = new Date('2000-01-01 ' + leaveTime);
                
                // Handle next day scenario
                if (leave < arrival) {
                    leave.setDate(leave.getDate() + 1);
                }
                
                const diffMs = leave - arrival;
                const hours = diffMs / (1000 * 60 * 60);
                
                document.getElementById('activityHours').value = hours.toFixed(1);
            }
        }

        function handlePlayerActivity(e) {
            e.preventDefault();
            
            const playerName = document.getElementById('activityPlayerName').value;
            const agentId = document.getElementById('activityAgentId').value;
            const gameSession = document.getElementById('activityGameSession').value;
            const arrivalTime = document.getElementById('activityArrival').value;
            const leaveTime = document.getElementById('activityLeave').value;
            const hoursPlayed = parseFloat(document.getElementById('activityHours').value);
            const rakeBack = parseFloat(document.getElementById('activityRakeBack').value);
            
            if (!playerName || !agentId || !gameSession || !arrivalTime || !leaveTime || !rakeBack) {
                alert('Please fill in all required fields');
                return;
            }
            
            const activity = {
                id: Date.now(),
                playerName,
                agentId,
                gameSession,
                arrivalTime,
                leaveTime,
                hoursPlayed,
                rakeBack,
                date: new Date().toLocaleDateString(),
                timestamp: new Date().toISOString()
            };
            
            // Save activity
            let activities = JSON.parse(localStorage.getItem('playerActivities') || '[]');
            activities.push(activity);
            localStorage.setItem('playerActivities', JSON.stringify(activities));
            
            // Reset form
            document.getElementById('playerActivityForm').reset();
            
            alert('Player activity recorded successfully! 📊');
        }

        function handleChangePassword(e) {
            e.preventDefault();
            
            const currentAgent = localStorage.getItem('currentAgent');
            const currentPassword = document.getElementById('currentPassword').value;
            const newPassword = document.getElementById('newPassword').value;
            const confirmPassword = document.getElementById('confirmNewPassword').value;
            
            if (newPassword !== confirmPassword) {
                alert('New passwords do not match!');
                return;
            }
            
            if (newPassword.length < 6) {
                alert('New password must be at least 6 characters long!');
                return;
            }
            
            // Get current agent data
            let agents = JSON.parse(localStorage.getItem('deployedAgents') || '[]');
            const agentIndex = agents.findIndex(a => a.id === currentAgent);
            
            if (agentIndex === -1) {
                alert('Agent not found!');
                return;
            }
            
            // Verify current password
            if (agents[agentIndex].password !== currentPassword) {
                alert('Current password is incorrect!');
                return;
            }
            
            // Update password
            agents[agentIndex].password = newPassword;
            localStorage.setItem('deployedAgents', JSON.stringify(agents));
            
            closeChangePasswordModal();
            alert('Password changed successfully! 🔑');
        }

        function showChangePasswordModal() {
            document.getElementById('changePasswordModal').classList.remove('hidden');
            document.getElementById('changePasswordModal').classList.add('flex');
        }

        function closeChangePasswordModal() {
            document.getElementById('changePasswordModal').classList.add('hidden');
            document.getElementById('changePasswordModal').classList.remove('flex');
            document.getElementById('changePasswordForm').reset();
        }

        function handleRegisterAgent(e) {
            e.preventDefault();
            
            const name = document.getElementById('registerAgentName').value;
            const phone = document.getElementById('registerAgentPhone').value;
            const staffId = document.getElementById('registerAgentStaffId').value;
            
            if (!name || !phone) return;
            
            let registeredAgents = JSON.parse(localStorage.getItem('registeredAgents') || '[]');
            
            // Check if agent already registered
            if (registeredAgents.some(a => a.phone === phone)) {
                alert('Agent with this phone number already registered!');
                return;
            }
            
            const newRegisteredAgent = {
                id: Date.now(),
                name: name,
                phone: phone,
                staffId: staffId || null,
                registered: new Date().toISOString(),
                deployed: false
            };
            
            registeredAgents.push(newRegisteredAgent);
            localStorage.setItem('registeredAgents', JSON.stringify(registeredAgents));
            
            document.getElementById('registerAgentForm').reset();
            loadRegisteredAgents();
            
            alert(`Agent registered successfully!\nName: ${name}\nPhone: ${phone}${staffId ? '\nStaff ID: ' + staffId : ''}`);
        }

        function handleDeployAgent(e) {
            e.preventDefault();
            
            const selectedAgentId = document.getElementById('selectRegisteredAgent').value;
            const loginId = document.getElementById('newAgentId').value;
            
            if (!selectedAgentId || !loginId) return;
            
            let registeredAgents = JSON.parse(localStorage.getItem('registeredAgents') || '[]');
            let deployedAgents = JSON.parse(localStorage.getItem('deployedAgents') || '[]');
            
            const registeredAgent = registeredAgents.find(a => a.id == selectedAgentId);
            if (!registeredAgent) {
                alert('Registered agent not found!');
                return;
            }
            
            if (deployedAgents.some(a => a.id === loginId)) {
                alert('Agent login ID already exists!');
                return;
            }
            
            const tempPassword = 'temp' + Math.random().toString(36).substr(2, 6);
            
            const newDeployedAgent = {
                id: loginId,
                name: registeredAgent.name,
                phone: registeredAgent.phone,
                staffId: registeredAgent.staffId,
                password: tempPassword,
                deployed: new Date().toISOString(),
                active: true,
                registeredId: registeredAgent.id
            };
            
            deployedAgents.push(newDeployedAgent);
            localStorage.setItem('deployedAgents', JSON.stringify(deployedAgents));
            
            // Mark registered agent as deployed
            registeredAgent.deployed = true;
            localStorage.setItem('registeredAgents', JSON.stringify(registeredAgents));
            
            document.getElementById('deployAgentForm').reset();
            loadActiveAgents();
            loadRegisteredAgents();
            updateAgentDropdown();
            
            alert(`Agent deployed successfully!\nLogin ID: ${loginId}\nTemporary Password: ${tempPassword}`);
        }

        function handlePlayerRegistration(e) {
            e.preventDefault();
            
            const name = document.getElementById('playerRealName').value;
            const phone = document.getElementById('playerPhoneNumber').value;
            const staffId = document.getElementById('playerStaffId').value;
            
            if (!name || !phone) return;
            
            let registeredPlayers = JSON.parse(localStorage.getItem('registeredPlayers') || '[]');
            
            // Check if player already registered
            if (registeredPlayers.some(p => p.phone === phone)) {
                alert('Player with this phone number already registered!');
                return;
            }
            
            const newPlayer = {
                id: Date.now(),
                name: name,
                phone: phone,
                staffId: staffId || null,
                registered: new Date().toISOString(),
                active: true
            };
            
            registeredPlayers.push(newPlayer);
            localStorage.setItem('registeredPlayers', JSON.stringify(registeredPlayers));
            
            document.getElementById('playerRegistrationForm').reset();
            loadRegisteredPlayers();
            
            alert(`Player registered successfully!\nName: ${name}\nPhone: ${phone}${staffId ? '\nStaff ID: ' + staffId : ''}`);
        }

        // Load agent data
        function loadAgentData(agentId) {
            // Get downline session records for this agent
            const sessionRecords = JSON.parse(localStorage.getItem('downlineSessionRecords') || '[]');
            const agentRecords = sessionRecords.filter(r => r.agentId === agentId);
            
            // Calculate totals
            const totalCommission = agentRecords.reduce((sum, r) => sum + r.commissionAmount, 0);
            const totalHours = agentRecords.reduce((sum, r) => sum + r.hoursPlayed, 0);
            const activeDownlines = new Set(agentRecords.map(r => r.playerName)).size;
            const totalSessions = agentRecords.length;
            
            // Update dashboard stats
            document.getElementById('agentTotalRakeBack').textContent = `$${totalCommission.toFixed(2)}`;
            document.getElementById('agentTotalHours').textContent = `${totalHours.toFixed(1)}h`;
            document.getElementById('agentActiveDownlines').textContent = activeDownlines;
            document.getElementById('agentTotalSessions').textContent = totalSessions;
            
            // Update downline activity
            const downlineContainer = document.getElementById('agentDownlineActivity');
            if (agentRecords.length === 0) {
                downlineContainer.innerHTML = '<p class="text-gray-400 text-center py-4">No downline activity recorded yet</p>';
            } else {
                // Group by player
                const playerStats = {};
                agentRecords.forEach(record => {
                    if (!playerStats[record.playerName]) {
                        playerStats[record.playerName] = {
                            totalHours: 0,
                            totalCommission: 0,
                            totalWinLoss: 0,
                            sessions: 0,
                            lastSession: record.date,
                            winSessions: 0,
                            loseSessions: 0
                        };
                    }
                    playerStats[record.playerName].totalHours += record.hoursPlayed;
                    playerStats[record.playerName].totalCommission += record.commissionAmount;
                    playerStats[record.playerName].totalWinLoss += record.winLossAmount;
                    playerStats[record.playerName].sessions += 1;
                    
                    if (record.playerResult === 'win') playerStats[record.playerName].winSessions++;
                    if (record.playerResult === 'lose') playerStats[record.playerName].loseSessions++;
                    
                    if (new Date(record.timestamp) > new Date(playerStats[record.playerName].lastSession)) {
                        playerStats[record.playerName].lastSession = record.date;
                    }
                });
                
                downlineContainer.innerHTML = Object.keys(playerStats).map(playerName => {
                    const stats = playerStats[playerName];
                    const winRate = stats.sessions > 0 ? ((stats.winSessions / stats.sessions) * 100).toFixed(1) : 0;
                    const winLossColor = stats.totalWinLoss >= 0 ? 'text-green-400' : 'text-red-400';
                    const winLossSign = stats.totalWinLoss >= 0 ? '+' : '';
                    
                    return `
                        <div class="bg-gray-600/30 rounded-lg p-4">
                            <div class="flex justify-between items-start mb-2">
                                <div>
                                    <p class="text-white font-medium">${playerName}</p>
                                    <p class="text-gray-400 text-sm">Last Session: ${stats.lastSession}</p>
                                </div>
                                <div class="text-right">
                                    <p class="text-green-400 font-bold">$${stats.totalCommission.toFixed(2)}</p>
                                    <p class="text-blue-400 text-sm">${stats.totalHours.toFixed(1)}h • ${stats.sessions} sessions</p>
                                </div>
                            </div>
                            <div class="flex justify-between items-center text-sm">
                                <div>
                                    <span class="text-green-300">${stats.winSessions}W</span> • 
                                    <span class="text-red-300">${stats.loseSessions}L</span> • 
                                    <span class="text-gray-300">${winRate}% Win Rate</span>
                                </div>
                                <div class="${winLossColor} font-medium">
                                    ${winLossSign}$${stats.totalWinLoss.toFixed(2)}
                                </div>
                            </div>
                        </div>
                    `;
                }).join('');
            }
            
            // Update recent sessions
            const recentContainer = document.getElementById('agentRecentSessions');
            const recentSessions = agentRecords
                .sort((a, b) => new Date(b.timestamp) - new Date(a.timestamp))
                .slice(0, 10);
                
            if (recentSessions.length === 0) {
                recentContainer.innerHTML = '<p class="text-gray-400 text-center py-4">No recent sessions</p>';
            } else {
                recentContainer.innerHTML = recentSessions.map(session => {
                    const resultIcon = session.playerResult === 'win' ? '🟢' : session.playerResult === 'lose' ? '🔴' : '🟡';
                    const winLossColor = session.winLossAmount >= 0 ? 'text-green-400' : 'text-red-400';
                    const winLossSign = session.winLossAmount >= 0 ? '+' : '';
                    
                    return `
                        <div class="bg-gray-600/30 rounded-lg p-3">
                            <div class="flex justify-between items-start mb-2">
                                <div>
                                    <p class="text-white font-medium">${session.playerName} ${resultIcon}</p>
                                    <p class="text-gray-400 text-sm">${session.gameSession}</p>
                                    <p class="text-gray-400 text-xs">${new Date(session.gameDate).toLocaleDateString()}</p>
                                    <p class="text-gray-400 text-xs">${session.startTime} - ${session.endTime}</p>
                                </div>
                                <div class="text-right">
                                    <p class="text-green-400 font-bold">$${session.commissionAmount.toFixed(2)}</p>
                                    <p class="text-blue-400 text-sm">${session.hoursPlayed.toFixed(1)} hours</p>
                                    <p class="${winLossColor} text-xs">${winLossSign}$${session.winLossAmount.toFixed(2)}</p>
                                </div>
                            </div>
                            ${session.notes ? `<p class="text-gray-300 text-xs italic">"${session.notes}"</p>` : ''}
                        </div>
                    `;
                }).join('');
            }
        }

        // Load member data
        function loadMemberData(username) {
            // Get member bookings
            const bookings = JSON.parse(localStorage.getItem('pokerBookings') || '[]');
            const memberBookings = bookings.filter(b => b.playerName.toLowerCase() === username.toLowerCase());
            
            // Get rake back records for this member
            const rakeBackRecords = JSON.parse(localStorage.getItem('rakeBackRecords') || '[]');
            const memberRecords = rakeBackRecords.filter(r => r.playerName.toLowerCase() === username.toLowerCase());
            
            // Calculate stats
            const totalBookings = memberBookings.length;
            const totalHours = memberRecords.reduce((sum, r) => sum + r.hoursPlayed, 0);
            const lastSession = memberRecords.length > 0 ? 
                new Date(Math.max(...memberRecords.map(r => new Date(r.timestamp)))).toLocaleDateString() : 
                'Never';
            
            // Update member stats
            document.getElementById('memberTotalBookings').textContent = totalBookings;
            document.getElementById('memberTotalHours').textContent = `${totalHours.toFixed(1)}h`;
            document.getElementById('memberLastSession').textContent = lastSession;
            
            // Update booking history
            const historyContainer = document.getElementById('memberBookingHistory');
            if (memberBookings.length === 0) {
                historyContainer.innerHTML = '<p class="text-gray-400 text-center py-4">No bookings yet</p>';
            } else {
                const recentBookings = memberBookings
                    .sort((a, b) => new Date(b.timestamp) - new Date(a.timestamp))
                    .slice(0, 10);
                    
                historyContainer.innerHTML = recentBookings.map(booking => `
                    <div class="bg-gray-600/30 rounded-lg p-4">
                        <div class="flex justify-between items-start">
                            <div>
                                <p class="text-white font-medium">${booking.gameSession || booking.gameDate}</p>
                                <p class="text-gray-400 text-sm">Arrival: ${booking.arrivalTime}</p>
                                <p class="text-gray-400 text-xs">Booked: ${new Date(booking.timestamp).toLocaleDateString()}</p>
                                ${booking.foodOrder ? `<p class="text-yellow-400 text-xs">🍽️ Food: ${booking.foodOrder}</p>` : ''}
                            </div>
                            <div class="text-right">
                                ${booking.seatReservation && booking.seatReservation.startsWith('25_') ? `<p class="text-green-400 text-sm">💺 Seat Reserved</p><p class="text-yellow-400 text-xs">🎰 Fee returns as chips</p>` : ''}
                                <p class="text-blue-400 text-xs">${booking.paymentStatus || 'No Payment'}</p>
                            </div>
                        </div>
                    </div>
                `).join('');
            }
        }

        // Load agent booking history
        function loadAgentBookingHistory() {
            const currentAgent = localStorage.getItem('currentUser');
            const currentAgentName = localStorage.getItem('currentUserName');
            
            // Get agent bookings
            const bookings = JSON.parse(localStorage.getItem('pokerBookings') || '[]');
            const agentBookings = bookings.filter(b => b.playerName === currentAgentName);
            
            // Update booking history
            const historyContainer = document.getElementById('agentBookingHistory');
            if (agentBookings.length === 0) {
                historyContainer.innerHTML = '<p class="text-gray-400 text-center py-4">No bookings yet</p>';
            } else {
                const recentBookings = agentBookings
                    .sort((a, b) => new Date(b.timestamp) - new Date(a.timestamp))
                    .slice(0, 10);
                    
                historyContainer.innerHTML = recentBookings.map(booking => `
                    <div class="bg-gray-600/30 rounded-lg p-4">
                        <div class="flex justify-between items-start">
                            <div>
                                <p class="text-white font-medium">${booking.gameSession || booking.gameDate}</p>
                                <p class="text-gray-400 text-sm">Arrival: ${booking.arrivalTime}</p>
                                <p class="text-gray-400 text-xs">Booked: ${new Date(booking.timestamp).toLocaleDateString()}</p>
                                ${booking.foodOrder ? `<p class="text-yellow-400 text-xs">🍽️ Food: ${booking.foodOrder}</p>` : ''}
                            </div>
                            <div class="text-right">
                                ${booking.seatReservation && booking.seatReservation.startsWith('25_') ? `<p class="text-green-400 text-sm">💺 Seat Reserved</p><p class="text-yellow-400 text-xs">🎰 Fee returns as chips</p>` : ''}
                                <p class="text-blue-400 text-xs">${booking.paymentStatus || 'No Payment'}</p>
                            </div>
                        </div>
                    </div>
                `).join('');
            }
        }

        // Logout function
        function logout() {
            document.getElementById('agentLogin').classList.remove('hidden');
            document.getElementById('agentDashboard').classList.add('hidden');
            document.getElementById('loginForm').reset();
            localStorage.removeItem('currentAgent');
        }

        // Close modal
        function closeModal() {
            document.getElementById('successModal').classList.add('hidden');
            document.getElementById('successModal').classList.remove('flex');
        }

        function adminLogout() {
            document.getElementById('adminLogin').classList.remove('hidden');
            document.getElementById('adminDashboard').classList.add('hidden');
            document.getElementById('adminLoginForm').reset();
            // Hide manage button when admin logs out
            document.getElementById('manageBtn').classList.add('hidden');
        }

        function showAdminTab(tab) {
            // Hide all tabs
            document.getElementById('scheduleTab').classList.add('hidden');
            document.getElementById('agentsTab').classList.add('hidden');
            document.getElementById('bookingsTab').classList.add('hidden');
            document.getElementById('playersTab').classList.add('hidden');
            
            // Reset button styles
            document.getElementById('scheduleTabBtn').className = 'px-4 py-2 bg-gray-600 text-white rounded-lg font-medium transition-all hover:bg-gray-500';
            document.getElementById('agentsTabBtn').className = 'px-4 py-2 bg-gray-600 text-white rounded-lg font-medium transition-all hover:bg-gray-500';
            document.getElementById('bookingsTabBtn').className = 'px-4 py-2 bg-gray-600 text-white rounded-lg font-medium transition-all hover:bg-gray-500';
            document.getElementById('playersTabBtn').className = 'px-4 py-2 bg-gray-600 text-white rounded-lg font-medium transition-all hover:bg-gray-500';
            
            // Show selected tab
            if (tab === 'schedule') {
                document.getElementById('scheduleTab').classList.remove('hidden');
                document.getElementById('scheduleTabBtn').className = 'px-4 py-2 bg-blue-600 text-white rounded-lg font-medium transition-all';
                loadScheduledGames();
            } else if (tab === 'agents') {
                document.getElementById('agentsTab').classList.remove('hidden');
                document.getElementById('agentsTabBtn').className = 'px-4 py-2 bg-blue-600 text-white rounded-lg font-medium transition-all';
                loadActiveAgents();
                loadRegisteredAgents();
            } else if (tab === 'bookings') {
                document.getElementById('bookingsTab').classList.remove('hidden');
                document.getElementById('bookingsTabBtn').className = 'px-4 py-2 bg-blue-600 text-white transition-all';
                loadRecentBookings();
            } else if (tab === 'players') {
                document.getElementById('playersTab').classList.remove('hidden');
                document.getElementById('playersTabBtn').className = 'px-4 py-2 bg-blue-600 text-white rounded-lg font-medium transition-all';
                loadRegisteredPlayers();
            }
        }

        function showAgentTab(tab) {
            // Hide all agent tabs
            document.getElementById('agentSessionsTab').classList.add('hidden');
            document.getElementById('agentBookingTab').classList.add('hidden');
            document.getElementById('agentHistoryTab').classList.add('hidden');
            
            // Reset button styles
            document.getElementById('agentSessionsTabBtn').className = 'px-4 py-2 bg-gray-600 text-white rounded-lg font-medium transition-all hover:bg-gray-500';
            document.getElementById('agentBookingTabBtn').className = 'px-4 py-2 bg-gray-600 text-white rounded-lg font-medium transition-all hover:bg-gray-500';
            document.getElementById('agentHistoryTabBtn').className = 'px-4 py-2 bg-gray-600 text-white rounded-lg font-medium transition-all hover:bg-gray-500';
            
            // Show selected tab
            if (tab === 'sessions') {
                document.getElementById('agentSessionsTab').classList.remove('hidden');
                document.getElementById('agentSessionsTabBtn').className = 'px-4 py-2 bg-blue-600 text-white rounded-lg font-medium transition-all';
            } else if (tab === 'booking') {
                document.getElementById('agentBookingTab').classList.remove('hidden');
                document.getElementById('agentBookingTabBtn').className = 'px-4 py-2 bg-blue-600 text-white rounded-lg font-medium transition-all';
            } else if (tab === 'history') {
                document.getElementById('agentHistoryTab').classList.remove('hidden');
                document.getElementById('agentHistoryTabBtn').className = 'px-4 py-2 bg-blue-600 text-white rounded-lg font-medium transition-all';
                loadAgentBookingHistory();
            }
        }

        function loadAdminData() {
            initializeAgents();
            initializeScheduledGames();
            loadScheduledGames();
            updateGameSessionDropdown();
            updateActivityAgentDropdown();
            updateActivityGameDropdown();
            // Show manage button for admin
            document.getElementById('manageBtn').classList.remove('hidden');
        }

        function updateActivityAgentDropdown() {
            const agents = JSON.parse(localStorage.getItem('deployedAgents') || '[]');
            const dropdown = document.getElementById('activityAgentId');
            
            if (dropdown) {
                dropdown.innerHTML = '<option value="">Select Agent</option>';
                
                agents.filter(agent => agent.active).forEach(agent => {
                    const option = document.createElement('option');
                    option.value = agent.id;
                    option.textContent = `${agent.name} (${agent.id})`;
                    dropdown.appendChild(option);
                });
            }
        }

        function updateActivityGameDropdown() {
            const scheduledGames = JSON.parse(localStorage.getItem('scheduledGames') || '[]');
            const dropdown = document.getElementById('activityGameSession');
            
            if (dropdown) {
                dropdown.innerHTML = '<option value="">Select Game</option>';
                
                scheduledGames.forEach(game => {
                    const option = document.createElement('option');
                    option.value = game.displayText;
                    option.textContent = game.displayText;
                    dropdown.appendChild(option);
                });
            }
        }

        // Game Management Functions
        function initializeScheduledGames() {
            // Always start with empty schedule - admin will add games manually
            if (!localStorage.getItem('scheduledGames')) {
                localStorage.setItem('scheduledGames', JSON.stringify([]));
            }
        }

        function updateGameSessionDropdown() {
            const scheduledGames = JSON.parse(localStorage.getItem('scheduledGames') || '[]');
            const dropdown = document.getElementById('gameSession');
            
            if (dropdown) {
                dropdown.innerHTML = '<option value="">Select Game Session</option>';
                
                scheduledGames.forEach(game => {
                    const option = document.createElement('option');
                    option.value = `${game.date}_${game.time}`;
                    option.textContent = game.displayText;
                    dropdown.appendChild(option);
                });
            }
        }

        function loadScheduledGames() {
            const scheduledGames = JSON.parse(localStorage.getItem('scheduledGames') || '[]');
            const container = document.getElementById('scheduledGamesList');
            
            if (!container) return;
            
            if (scheduledGames.length === 0) {
                container.innerHTML = '<p class="text-gray-400 text-center py-4">No games scheduled yet</p>';
                return;
            }
            
            container.innerHTML = scheduledGames.map((game, index) => `
                <div class="flex justify-between items-center bg-gray-600/30 rounded-lg p-4">
                    <div>
                        <p class="text-white font-medium">${game.displayText}</p>
                        <p class="text-gray-400 text-sm">Game ID: ${game.id}</p>
                    </div>
                    <button onclick="removeScheduledGame(${index})" class="bg-red-600 hover:bg-red-700 text-white px-3 py-1 rounded-lg text-sm transition-all">
                        Remove
                    </button>
                </div>
            `).join('');
        }

        function removeScheduledGame(index) {
            let scheduledGames = JSON.parse(localStorage.getItem('scheduledGames') || '[]');
            scheduledGames.splice(index, 1);
            localStorage.setItem('scheduledGames', JSON.stringify(scheduledGames));
            loadScheduledGames();
            updateGameSessionDropdown();
            loadScheduleDisplay();
        }

        // Agent Management Functions
        function initializeAgents() {
            let agents = JSON.parse(localStorage.getItem('deployedAgents') || '[]');
            if (agents.length === 0) {
                agents = [
                    { id: 'agent1', name: 'Mike Chen', password: 'poker123', deployed: new Date().toISOString(), active: true },
                    { id: 'agent2', name: 'Sarah Johnson', password: 'poker123', deployed: new Date().toISOString(), active: true },
                    { id: 'agent3', name: 'David Rodriguez', password: 'poker123', deployed: new Date().toISOString(), active: true },
                    { id: 'agent4', name: 'Lisa Wang', password: 'poker123', deployed: new Date().toISOString(), active: true }
                ];
                localStorage.setItem('deployedAgents', JSON.stringify(agents));
            }
            updateAgentDropdown();
        }

        function updateAgentDropdown() {
            const agents = JSON.parse(localStorage.getItem('deployedAgents') || '[]');
            const dropdown = document.getElementById('referringAgent');
            
            if (dropdown) {
                dropdown.innerHTML = '<option value="">Select Agent</option>';
                
                agents.filter(agent => agent.active).forEach(agent => {
                    const option = document.createElement('option');
                    option.value = agent.id;
                    option.textContent = agent.name;
                    dropdown.appendChild(option);
                });
            }
        }

        function loadActiveAgents() {
            const agents = JSON.parse(localStorage.getItem('deployedAgents') || '[]');
            const container = document.getElementById('activeAgentsList');
            
            if (!container) return;
            
            if (agents.length === 0) {
                container.innerHTML = '<p class="text-gray-400 text-center py-4">No agents deployed yet</p>';
                return;
            }
            
            container.innerHTML = agents.map((agent, index) => `
                <div class="flex justify-between items-center bg-gray-600/30 rounded-lg p-4">
                    <div>
                        <p class="text-white font-medium">${agent.name}</p>
                        <p class="text-gray-400 text-sm">ID: ${agent.id} | Password: ${agent.password}</p>
                        <p class="text-gray-400 text-xs">Deployed: ${new Date(agent.deployed).toLocaleDateString()}</p>
                    </div>
                    <div class="flex space-x-2">
                        <span class="px-2 py-1 rounded text-xs ${agent.active ? 'bg-green-600 text-white' : 'bg-red-600 text-white'}">
                            ${agent.active ? 'Active' : 'Inactive'}
                        </span>
                        <button onclick="toggleAgent(${index})" class="bg-yellow-600 hover:bg-yellow-700 text-white px-3 py-1 rounded-lg text-sm transition-all">
                            ${agent.active ? 'Deactivate' : 'Activate'}
                        </button>
                        <button onclick="resetAgentPassword(${index})" class="bg-blue-600 hover:bg-blue-700 text-white px-3 py-1 rounded-lg text-sm transition-all">
                            Reset Password
                        </button>
                        <button onclick="deleteAgent(${index})" class="bg-red-600 hover:bg-red-700 text-white px-3 py-1 rounded-lg text-sm transition-all">
                            Delete
                        </button>
                    </div>
                </div>
            `).join('');
        }

        function toggleAgent(index) {
            let agents = JSON.parse(localStorage.getItem('deployedAgents') || '[]');
            agents[index].active = !agents[index].active;
            localStorage.setItem('deployedAgents', JSON.stringify(agents));
            loadActiveAgents();
            updateAgentDropdown();
        }

        function resetAgentPassword(index) {
            let agents = JSON.parse(localStorage.getItem('deployedAgents') || '[]');
            const newPassword = 'temp' + Math.random().toString(36).substr(2, 6);
            agents[index].password = newPassword;
            localStorage.setItem('deployedAgents', JSON.stringify(agents));
            loadActiveAgents();
            alert(`New password for ${agents[index].name}: ${newPassword}`);
        }

        function deleteAgent(index) {
            let agents = JSON.parse(localStorage.getItem('deployedAgents') || '[]');
            const agentName = agents[index].name;
            
            if (confirm(`Are you sure you want to delete agent "${agentName}"? This action cannot be undone.`)) {
                agents.splice(index, 1);
                localStorage.setItem('deployedAgents', JSON.stringify(agents));
                loadActiveAgents();
                updateAgentDropdown();
                alert(`Agent "${agentName}" has been deleted successfully.`);
            }
        }

        function loadRecentBookings() {
            const bookings = JSON.parse(localStorage.getItem('pokerBookings') || '[]');
            const container = document.getElementById('recentBookingsList');
            
            if (!container) return;
            
            if (bookings.length === 0) {
                container.innerHTML = '<p class="text-gray-400 text-center py-4">No bookings yet</p>';
                return;
            }
            
            const recentBookings = bookings.sort((a, b) => new Date(b.timestamp) - new Date(a.timestamp)).slice(0, 20);
            
            container.innerHTML = recentBookings.map(booking => `
                <div class="bg-gray-600/30 rounded-lg p-4">
                    <div class="flex justify-between items-start">
                        <div>
                            <p class="text-white font-medium">${booking.playerName}</p>
                            <p class="text-gray-400 text-sm">${booking.gameSession || booking.gameDate} - ${booking.gameTime}</p>
                            <p class="text-gray-400 text-xs">Booked: ${new Date(booking.timestamp).toLocaleString()}</p>
                            ${booking.foodOrder ? `<p class="text-yellow-400 text-xs">🍽️ Food: ${booking.foodOrder}</p>` : ''}
                        </div>
                        <div class="text-right">
                            ${booking.seatReservation && booking.seatReservation.startsWith('25_') ? `<p class="text-green-400 text-sm">💺 Seat Reserved</p><p class="text-yellow-400 text-xs">🎰 Fee returns as chips</p>` : ''}
                            ${booking.agent ? `<p class="text-blue-400 text-xs">Agent: ${booking.agent}</p>` : ''}
                        </div>
                    </div>
                </div>
            `).join('');
        }

        // Load schedule display
        function loadScheduleDisplay() {
            const scheduledGames = JSON.parse(localStorage.getItem('scheduledGames') || '[]');
            const container = document.getElementById('scheduleDisplay');
            
            if (!container) return;
            
            if (scheduledGames.length === 0) {
                container.innerHTML = `
                    <div class="text-center py-12">
                        <div class="text-6xl mb-4">📅</div>
                        <h3 class="text-2xl font-bold text-white mb-4">No Games Scheduled</h3>
                        <p class="text-gray-300 mb-6">Contact admin to schedule games</p>
                        <div class="bg-gray-700/30 rounded-lg p-4 max-w-md mx-auto">
                            <p class="text-gray-300 text-sm">🔐 Admin access required to manage schedule</p>
                        </div>
                    </div>
                `;
                return;
            }
            
            // Display only the games that have been created by admin
            let html = '<div class="grid md:grid-cols-1 lg:grid-cols-2 gap-6">';
            
            // Sort games by date and time
            const sortedGames = scheduledGames.sort((a, b) => {
                const dateA = new Date(a.date + ' ' + a.time);
                const dateB = new Date(b.date + ' ' + b.time);
                return dateA - dateB;
            });
            
            sortedGames.forEach(game => {
                const gameDate = new Date(game.date + ' ' + game.time);
                const isUpcoming = gameDate > new Date();
                const isPast = gameDate < new Date();
                
                let statusColor = 'blue';
                let statusText = 'Scheduled';
                
                if (isPast) {
                    statusColor = 'gray';
                    statusText = 'Completed';
                } else if (isUpcoming) {
                    const hoursUntil = (gameDate - new Date()) / (1000 * 60 * 60);
                    if (hoursUntil < 24) {
                        statusColor = 'yellow';
                        statusText = 'Starting Soon';
                    } else {
                        statusColor = 'green';
                        statusText = 'Upcoming';
                    }
                }
                
                const colorClasses = {
                    blue: 'from-blue-600/20 to-blue-800/20 border-blue-500/30 text-blue-300',
                    green: 'from-green-600/20 to-green-800/20 border-green-500/30 text-green-300',
                    yellow: 'from-yellow-600/20 to-yellow-800/20 border-yellow-500/30 text-yellow-300',
                    gray: 'from-gray-600/20 to-gray-800/20 border-gray-500/30 text-gray-300'
                };
                
                const colors = colorClasses[statusColor];
                
                html += `
                    <div class="bg-gradient-to-br ${colors} p-6 rounded-xl border">
                        <div class="flex justify-between items-start mb-4">
                            <div>
                                <h3 class="text-xl font-bold text-white mb-2">${game.day}</h3>
                                <p class="text-lg text-gray-300">${new Date(game.date).toLocaleDateString()}</p>
                                <p class="text-2xl font-bold text-white">${new Date('2000-01-01 ' + game.time).toLocaleTimeString('en-US', { hour: 'numeric', minute: '2-digit', hour12: true })}</p>
                            </div>
                            <span class="px-3 py-1 rounded-full text-xs font-medium bg-white/20 text-white">
                                ${statusText}
                            </span>
                        </div>
                        
                        <div class="bg-white/10 rounded-lg p-4">
                            <div class="grid grid-cols-2 gap-4 text-sm">
                                <div>
                                    <p class="text-gray-300">Game ID</p>
                                    <p class="text-white font-medium">${game.id}</p>
                                </div>
                                <div>
                                    <p class="text-gray-300">Status</p>
                                    <p class="text-white font-medium">${statusText}</p>
                                </div>
                            </div>
                        </div>
                    </div>
                `;
            });
            
            html += '</div>';
            container.innerHTML = html;
        }

        function loadScheduledDates() {
            // This function can be used for additional loading when manage section is opened
            loadScheduledGames();
        }

        function loadRegisteredAgents() {
            const registeredAgents = JSON.parse(localStorage.getItem('registeredAgents') || '[]');
            const dropdown = document.getElementById('selectRegisteredAgent');
            
            if (dropdown) {
                dropdown.innerHTML = '<option value="">Select Agent to Deploy</option>';
                
                registeredAgents.filter(agent => !agent.deployed).forEach(agent => {
                    const option = document.createElement('option');
                    option.value = agent.id;
                    option.textContent = `${agent.name} - ${agent.phone}${agent.staffId ? ' (' + agent.staffId + ')' : ''}`;
                    dropdown.appendChild(option);
                });
            }
        }

        function loadRegisteredPlayers() {
            const registeredPlayers = JSON.parse(localStorage.getItem('registeredPlayers') || '[]');
            const container = document.getElementById('registeredPlayersList');
            
            if (!container) return;
            
            if (registeredPlayers.length === 0) {
                container.innerHTML = '<p class="text-gray-400 text-center py-4">No players registered yet</p>';
                return;
            }
            
            container.innerHTML = registeredPlayers.map((player, index) => `
                <div class="flex justify-between items-center bg-gray-600/30 rounded-lg p-4">
                    <div>
                        <p class="text-white font-medium">${player.name}</p>
                        <p class="text-gray-400 text-sm">Phone: ${player.phone}</p>
                        ${player.staffId ? `<p class="text-gray-400 text-xs">Staff ID: ${player.staffId}</p>` : ''}
                        <p class="text-gray-400 text-xs">Registered: ${new Date(player.registered).toLocaleDateString()}</p>
                    </div>
                    <div class="flex space-x-2">
                        <span class="px-2 py-1 rounded text-xs ${player.active ? 'bg-green-600 text-white' : 'bg-red-600 text-white'}">
                            ${player.active ? 'Active' : 'Inactive'}
                        </span>
                        <button onclick="togglePlayer(${index})" class="bg-yellow-600 hover:bg-yellow-700 text-white px-3 py-1 rounded-lg text-sm transition-all">
                            ${player.active ? 'Deactivate' : 'Activate'}
                        </button>
                    </div>
                </div>
            `).join('');
        }

        function togglePlayer(index) {
            let registeredPlayers = JSON.parse(localStorage.getItem('registeredPlayers') || '[]');
            registeredPlayers[index].active = !registeredPlayers[index].active;
            localStorage.setItem('registeredPlayers', JSON.stringify(registeredPlayers));
            loadRegisteredPlayers();
        }
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'97c2c3a2478a3c6f',t:'MTc1NzM3OTc4OS4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
