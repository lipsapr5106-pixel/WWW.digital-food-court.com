<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Smart Food Court | Lipsa Pr</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        .glass { background: rgba(255, 255, 255, 0.9); backdrop-filter: blur(10px); }
        .hero-gradient { background: linear-gradient(135deg, #ff6b6b 0%, #ff8e53 100%); }
    </style>
</head>
<body class="bg-gray-100 font-sans">

    <nav class="glass sticky top-0 z-50 shadow-sm border-b border-gray-200">
        <div class="max-w-7xl mx-auto px-6 py-4 flex justify-between items-center">
            <div class="flex items-center gap-2">
                <i class="fa-solid fa-utensils text-orange-500 text-2xl"></i>
                <h1 class="text-xl font-bold text-gray-800 tracking-tight">Digital<span class="text-orange-500">FoodCourt</span></h1>
            </div>
            <div class="hidden md:flex gap-8 font-medium text-gray-600">
                <a href="#home" class="hover:text-orange-500">Home</a>
                <a href="#menu" class="hover:text-orange-500">Menu</a>
                <a href="#tracking" class="hover:text-orange-500">Track Order</a>
            </div>
            <button class="bg-orange-500 text-white px-6 py-2 rounded-full font-semibold hover:bg-orange-600 transition shadow-lg shadow-orange-200">
                Cart (0)
            </button>
        </div>
    </nav>

    <section id="home" class="hero-gradient text-white py-20 px-6">
        <div class="max-w-7xl mx-auto text-center">
            <h2 class="text-4xl md:text-6xl font-extrabold mb-6">Skip the Queue, <br>Order Digitally.</h2>
            <p class="text-lg opacity-90 mb-8 max-w-2xl mx-auto">Reduce waiting time and enjoy a modern food ordering experience with real-time tracking.</p>
            <div class="flex flex-wrap justify-center gap-4">
                <a href="#menu" class="bg-white text-orange-600 px-8 py-3 rounded-xl font-bold hover:bg-gray-100 transition">View Menu</a>
                <button class="border-2 border-white px-8 py-3 rounded-xl font-bold hover:bg-white hover:text-orange-600 transition">Our Features</button>
            </div>
        </div>
    </section>

    <section class="max-w-7xl mx-auto py-16 px-6">
        <h3 class="text-3xl font-bold text-center mb-12 text-gray-800">Why Digital Food Court?</h3>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8 text-center">
            <div class="bg-white p-8 rounded-2xl shadow-sm border border-gray-100">
                <i class="fa-solid fa-bolt text-4xl text-yellow-500 mb-4"></i>
                <h4 class="text-xl font-bold mb-2">Saves Time</h4>
                <p class="text-gray-500">No more standing in long queues at the counter.</p>
            </div>
            <div class="bg-white p-8 rounded-2xl shadow-sm border border-gray-100">
                <i class="fa-solid fa-credit-card text-4xl text-green-500 mb-4"></i>
                <h4 class="text-xl font-bold mb-2">Secure Payment</h4>
                <p class="text-gray-500">Multiple online payment options like UPI & Cards.</p>
            </div>
            <div class="bg-white p-8 rounded-2xl shadow-sm border border-gray-100">
                <i class="fa-solid fa-clock-rotate-left text-4xl text-blue-500 mb-4"></i>
                <h4 class="text-xl font-bold mb-2">Live Tracking</h4>
                <p class="text-gray-500">Know exactly when your food is ready to pick up.</p>
            </div>
        </div>
    </section>

    <section id="menu" class="bg-gray-50 py-16 px-6">
        <div class="max-w-7xl mx-auto">
            <div class="flex justify-between items-end mb-10">
                <div>
                    <h3 class="text-3xl font-bold text-gray-800">Explore Menu</h3>
                    <p class="text-gray-500">From multiple stalls in one place</p>
                </div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
                <div class="bg-white rounded-2xl shadow-md overflow-hidden group">
                    <img src="https://images.unsplash.com/photo-1568901346375-23c9450c58cd?w=500" class="h-48 w-full object-cover group-hover:scale-105 transition duration-300">
                    <div class="p-5">
                        <span class="text-xs font-bold text-orange-500 bg-orange-50 px-2 py-1 rounded">BURGER HUB</span>
                        <h4 class="font-bold text-lg mt-2 text-gray-800">Classic Cheese Burger</h4>
                        <div class="flex justify-between items-center mt-4">
                            <span class="font-bold text-xl text-gray-900">₹149</span>
                            <button onclick="orderPlaced()" class="bg-gray-900 text-white px-4 py-2 rounded-lg text-sm font-semibold hover:bg-orange-500 transition">Add To Cart</button>
                        </div>
                    </div>
                </div>

                <div class="bg-white rounded-2xl shadow-md overflow-hidden group">
                    <img src="https://images.unsplash.com/photo-1513104890138-7c749659a591?w=500" class="h-48 w-full object-cover group-hover:scale-105 transition duration-300">
                    <div class="p-5">
                        <span class="text-xs font-bold text-orange-500 bg-orange-50 px-2 py-1 rounded">PIZZA CORNER</span>
                        <h4 class="font-bold text-lg mt-2 text-gray-800">Paneer Tikka Pizza</h4>
                        <div class="flex justify-between items-center mt-4">
                            <span class="font-bold text-xl text-gray-900">₹299</span>
                            <button onclick="orderPlaced()" class="bg-gray-900 text-white px-4 py-2 rounded-lg text-sm font-semibold hover:bg-orange-500 transition">Add To Cart</button>
                        </div>
                    </div>
                </div>

                <div class="bg-white rounded-2xl shadow-md overflow-hidden group">
                    <img src="https://images.unsplash.com/photo-1546833999-b9f581a1996d?w=500" class="h-48 w-full object-cover group-hover:scale-105 transition duration-300">
                    <div class="p-5">
                        <span class="text-xs font-bold text-orange-500 bg-orange-50 px-2 py-1 rounded">ODIA KITCHEN</span>
                        <h4 class="font-bold text-lg mt-2 text-gray-800">Special Veg Thali</h4>
                        <div class="flex justify-between items-center mt-4">
                            <span class="font-bold text-xl text-gray-900">₹180</span>
                            <button onclick="orderPlaced()" class="bg-gray-900 text-white px-4 py-2 rounded-lg text-sm font-semibold hover:bg-orange-500 transition">Add To Cart</button>
                        </div>
                    </div>
                </div>

                <div class="bg-white rounded-2xl shadow-md overflow-hidden group">
                    <img src="https://images.unsplash.com/photo-1546173159-315724a31696?w=500" class="h-48 w-full object-cover group-hover:scale-105 transition duration-300">
                    <div class="p-5">
                        <span class="text-xs font-bold text-orange-500 bg-orange-50 px-2 py-1 rounded">BEVERAGE BAR</span>
                        <h4 class="font-bold text-lg mt-2 text-gray-800">Mango Lassi</h4>
                        <div class="flex justify-between items-center mt-4">
                            <span class="font-bold text-xl text-gray-900">₹80</span>
                            <button onclick="orderPlaced()" class="bg-gray-900 text-white px-4 py-2 rounded-lg text-sm font-semibold hover:bg-orange-500 transition">Add To Cart</button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="tracking" class="py-16 px-6 max-w-4xl mx-auto text-center">
        <div class="bg-white p-10 rounded-3xl shadow-xl border border-orange-100">
            <h3 class="text-2xl font-bold mb-6">Order Status</h3>
            <div id="statusBox" class="flex flex-col items-center gap-4">
                <div class="flex gap-4 items-center mb-6">
                    <div class="w-12 h-12 bg-green-500 text-white rounded-full flex items-center justify-center">1</div>
                    <div class="h-1 w-16 bg-green-500"></div>
                    <div id="step2" class="w-12 h-12 bg-gray-200 text-gray-500 rounded-full flex items-center justify-center">2</div>
                    <div class="h-1 w-16 bg-gray-200"></div>
                    <div id="step3" class="w-12 h-12 bg-gray-200 text-gray-500 rounded-full flex items-center justify-center">3</div>
                </div>
                <p id="statusText" class="text-xl font-medium text-gray-700 italic">"Waiting for your order..."</p>
            </div>
        </div>
    </section>

    <footer class="bg-gray-900 text-white py-12 px-6 text-center">
        <p class="text-orange-500 font-bold mb-2">B.Tech Mini Project</p>
        <p class="text-lg mb-1">Presented by: <b>Lipsa Pr</b></p>
        <p class="opacity-50 text-sm">© 2026 Digital Food Court System. All Rights Reserved.</p>
    </footer>

    <script>
        function orderPlaced() {
            const statusText = document.getElementById('statusText');
            const step2 = document.getElementById('step2');
            const step3 = document.getElementById('step3');

            statusText.innerText = "Order Received! Kitchen is preparing...";
            statusText.classList.add('text-orange-500');

            setTimeout(() => {
                step2.classList.replace('bg-gray-200', 'bg-green-500');
                step2.classList.replace('text-gray-500', 'text-white');
                statusText.innerText = "Your food is being cooked! 👨‍🍳";
            }, 3000);

            setTimeout(() => {
                step3.classList.replace('bg-gray-200', 'bg-green-500');
                step3.classList.replace('text-gray-500', 'text-white');
                statusText.innerText = "Order Ready! Please collect from Stall. ✅";
                alert("Payment Successful! Order ID: #DFC2026");
            }, 7000);
        }
    </script>
</body>
</html>
