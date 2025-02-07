<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Doc Connect</title>
    <meta name="description" content="Connect with the right healthcare professional for your needs with seamless appointment booking and secure payment processing">
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
    <link href="https://cdn.jsdelivr.net/npm/@tailwindcss/typography/dist/typography.min.css" rel="stylesheet">
    <script src="https://unpkg.com/vue@3.5.13/dist/vue.global.js"></script>
</head>
<body class="bg-gray-50">
    <div id="app" class="min-h-screen">
        <!-- Login Page -->
        <div v-if="currentPage === 'login'" class="min-h-screen flex items-center justify-center">
            <div class="max-w-md w-full bg-white rounded-lg shadow-md p-8">
                <div class="text-center mb-8">
                    <h1 class="text-2xl font-bold text-blue-600">Doc Connect</h1>
                    <p class="text-gray-600 mt-2">Your Healthcare Partner</p>
                </div>
                <form @submit.prevent="login" class="space-y-6">
                    <div>
                        <label class="block text-gray-700 mb-2">Phone Number</label>
                        <input type="tel" v-model="phoneNumber" required pattern="[0-9]{10}" class="w-full px-4 py-2 border rounded-lg" placeholder="Enter 10 digit number">
                    </div>
                    <button v-if="!otpSent" @click.prevent="sendOTP" class="w-full bg-blue-600 text-white py-2 rounded-lg hover:bg-blue-700 transition-colors">Send OTP</button>
                    <div v-if="otpSent">
                        <label class="block text-gray-700 mb-2">Enter OTP</label>
                        <input type="text" v-model="otp" required pattern="[0-9]{4}" maxlength="4" class="w-full px-4 py-2 border rounded-lg" placeholder="Enter 4 digit OTP">
                        <p class="text-sm text-gray-500 mt-1">OTP valid for 10 minutes</p>
                        <p v-if="otpError" class="text-red-500 text-sm mt-1">{{ otpError }}</p>
                    </div>
                    <button type="submit" class="w-full bg-blue-600 text-white py-2 rounded-lg hover:bg-blue-700 transition-colors">
                        Login
                    </button>
                </form>
                <p class="text-center mt-4 text-gray-600">
                    New user? <a href="#" class="text-blue-600">Sign up</a>
                </p>
            </div>
        </div>

        <!-- Main Navigation after login -->
        <header v-if="isLoggedIn" class="bg-white shadow-sm">
            <nav class="container mx-auto px-4 py-4">
                <div class="flex justify-between items-center">
                    <div class="flex items-center">
                        <span class="text-xl font-bold text-blue-600">Doc Connect</span>
                    </div>
                    <div class="flex space-x-4">
                        <button @click="currentPage = 'about'" class="text-gray-600 hover:text-blue-600">About Us</button>
                        <button @click="currentPage = 'history'" class="text-gray-600 hover:text-blue-600">Consultation History</button>
                        <button @click="currentPage = 'doctors'" class="text-gray-600 hover:text-blue-600">Find Doctors</button>
                        <button @click="logout" class="text-gray-600 hover:text-blue-600">Logout</button>
                    </div>
                </div>
            </nav>
        </header>

        <main class="container mx-auto px-4 py-8">
            <!-- About Us Page -->
            <div v-if="currentPage === 'about'" class="max-w-4xl mx-auto prose">
                <h2 class="text-2xl font-bold mb-6">About Us</h2>
                <div class="space-y-6">
                    <p>Welcome to DocConnect, your trusted partner in managing your healthcare needs conveniently and efficiently. At DocConnect, we understand the challenges individuals face when it comes to scheduling doctor appointments and managing their health records.</p>
                    
                    <p>DocConnect is committed to excellence in healthcare technology. We continuously strive to enhance our platform, integrating the latest advancements to improve user experience and deliver superior service. Whether you're booking your first appointment or managing ongoing care, DocConnect is here to support you every step of the way.</p>
                    
                    <h3 class="text-xl font-semibold">Our Vision</h3>
                    <p>Our vision at DocConnect is to create a seamless healthcare experience for every user. We aim to bridge the gap between patients and healthcare providers, making it easier for you to access the care you need, when you need it.</p>
                    
                    <h3 class="text-xl font-bold mt-6">Contact Us</h3>
                    <p class="font-bold">Phone: 8107789136</p>
                </div>
            </div>
            <!-- Consultation History Page -->
            <div v-if="currentPage === 'history'" class="max-w-4xl mx-auto">
                <h2 class="text-2xl font-bold mb-6">Consultation History</h2>
                <div class="mb-6">
                    <label class="block mb-2">Upload Medical Records/Reports</label>
                    <input type="file" @change="handleFileUpload" accept="image/*" multiple class="w-full p-2 border rounded-lg">
                </div>
                <div class="space-y-4">
                    <div v-for="(record, index) in consultationHistory" :key="index" class="border rounded-lg p-4">
                        <div class="flex justify-between items-start">
                            <div>
                                <h4 class="font-semibold">{{ record.date }}</h4>
                                <p class="text-gray-600">{{ record.doctor }}</p>
                                <p class="mt-2">{{ record.notes }}</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Doctors Page -->
            <div v-if="currentPage === 'doctors'" class="max-w-4xl mx-auto">
                <h2 class="text-2xl font-bold mb-6">Available Doctors</h2>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                    <div class="bg-white p-6 rounded-lg shadow-md">
                        <h3 class="text-xl font-semibold">Dr. M.V. Kamalakar</h3>
                        <p class="text-gray-600">Family Physician & Geriatric Specialist</p>
                        <button @click="openBooking('Dr. M.V. Kamalakar')" class="mt-4 bg-blue-600 text-white px-4 py-2 rounded-lg hover:bg-blue-700">
                            Book Appointment
                        </button>
                    </div>
                    <div class="bg-white p-6 rounded-lg shadow-md">
                        <h3 class="text-xl font-semibold">Dr. Raghvendra Bagla</h3>
                        <p class="text-gray-600">Family Physician</p>
                        <button @click="openBooking('Dr. Raghvendra Bagla')" class="mt-4 bg-blue-600 text-white px-4 py-2 rounded-lg hover:bg-blue-700">
                            Book Appointment
                        </button>
                    </div>
                </div>
                <!-- Booking Modal -->
                <div v-if="showBookingModal" class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center">
                    <div class="bg-white p-6 rounded-lg max-w-md w-full">
                        <button @click="closeBooking" class="absolute top-2 right-2 text-gray-500 hover:text-gray-700">
                            <span class="text-xl">&times;</span>
                        </button>
                        <h3 class="text-xl font-semibold mb-4">Book Appointment with {{selectedDoctor}}</h3>
                        <div class="mb-4">
                            <label class="block text-gray-700 mb-2">Select Date</label>
                            <input type="date" v-model="selectedDate" class="w-full px-4 py-2 border rounded-lg">
                        </div>
                        <div class="mb-4" v-if="selectedDate">
                            <label class="block text-gray-700 mb-2">Select Time</label>
                            <select v-model="selectedTime" class="w-full px-4 py-2 border rounded-lg">
                                <option value="09:00">09:00 AM</option>
                                <option value="10:00">10:00 AM</option>
                                <option value="11:00">11:00 AM</option>
                                <option value="12:00">12:00 PM</option>
                                <option value="14:00">02:00 PM</option>
                                <option value="15:00">03:00 PM</option>
                                <option value="16:00">04:00 PM</option>
                            </select>
                        </div>
                        <div v-if="selectedTime" class="mb-4">
                            <h4 class="font-semibold mb-2">Payment Details</h4>
                            <p class="mb-2">Consultation Fee: ₹200</p>
                            <img :src="selectedDoctor === 'Dr. Raghvendra Bagla' ? 'qr-bagla.png' : 'qr-kamalakar.png'" alt="Payment QR Code" class="mx-auto mb-2">
                            <p class="text-sm text-gray-600">Scan QR code to pay</p>
                            <p class="text-sm text-gray-600">Mobile: {{selectedDoctor === 'Dr. Raghvendra Bagla' ? '9717746498' : '8107789136'}}</p>
                        </div>
                        <div class="flex justify-end space-x-2">
                            <button @click="closeBooking" class="px-4 py-2 text-gray-600 hover:text-gray-800">Cancel</button>
                            <button @click="confirmBooking" v-if="selectedTime" class="px-4 py-2 bg-blue-600 text-white rounded-lg hover:bg-blue-700">
                                Confirm Booking
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </main>
    </div>

    <script type="module">
        const { createApp, ref } = Vue;

        createApp({
            setup() {
                const currentPage = ref('login');
                const isLoggedIn = ref(false);
                const phoneNumber = ref('');
                const otp = ref('');
                const otpSent = ref(false);
                const otpError = ref('');
                const generatedOTP = ref('');
                const otpTimestamp = ref(null);
                const patientData = ref({});
                const showBookingModal = ref(false);
                const selectedDoctor = ref('');
                const selectedDate = ref('');
                const selectedTime = ref('');
                const consultationHistory = ref([]);

                const sendOTP = () => {
                    // Generate a random 4-digit OTP
                    generatedOTP.value = Math.floor(1000 + Math.random() * 9000).toString();
                    otpTimestamp.value = new Date();
                    otpSent.value = true;
                    alert(`Your OTP is: ${generatedOTP.value}`); // In a real app, this would be sent via SMS
                };

                const login = () => {
                    const currentTime = new Date();
                    const timeDiff = (currentTime - otpTimestamp.value) / 1000 / 60; // time difference in minutes
                    
                    if (timeDiff > 10) {
                        otpError.value = 'OTP has expired. Please request a new one.';
                        return;
                    }

                    if (otp.value !== generatedOTP.value) {
                        otpError.value = 'Invalid OTP. Please try again.';
                        return;
                    }

                    // Store patient phone for personalized access
                    patientData.value = {
                        phone: phoneNumber.value,
                        consultationHistory: [],
                        appointments: []
                    };
                    isLoggedIn.value = true;
                    currentPage.value = 'doctors';
                };

                const openBooking = (doctor) => {
                    selectedDoctor.value = doctor;
                    showBookingModal.value = true;
                    selectedDate.value = '';
                    selectedTime.value = '';
                };

                const closeBooking = () => {
                    showBookingModal.value = false;
                };

                const confirmBooking = () => {
                    let doctorContact = '';
                    if (selectedDoctor.value === 'Dr. Raghvendra Bagla') {
                        doctorContact = '9717746498';
                    } else if (selectedDoctor.value === 'Dr. M.V. Kamalakar') {
                        doctorContact = '8107789136';
                    }
                    alert(`Appointment confirmed with ${selectedDoctor.value} for ${selectedDate.value} at ${selectedTime.value}. Notification sent to doctor at ${doctorContact}`);
                    closeBooking();
                };

                const logout = () => {
                    isLoggedIn.value = false;
                    currentPage.value = 'login';
                };

                const handleFileUpload = (event) => {
                    // Store files in patient's personal records
                    patientData.value.consultationHistory.push(event.target.files);
                    // Handle file upload logic here
                };

                return {
                    currentPage,
                    isLoggedIn,
                    phoneNumber,
                    otp,
                    otpSent,
                    otpError,
                    sendOTP,
                    patientData,
                    showBookingModal,
                    selectedDoctor,
                    selectedDate,
                    selectedTime,
                    consultationHistory,
                    login,
                    logout,
                    handleFileUpload,
                    openBooking,
                    closeBooking,
                    confirmBooking
                };
            }
        }).mount('#app');
    </script>
</body>
</html>
