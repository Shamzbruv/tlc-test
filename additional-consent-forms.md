<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Additional Consent Forms - TLC Family Services</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@500;600;700&family=Lato:wght@300;400;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        .font-serif {
            font-family: 'Cormorant Garamond', serif;
        }
        .font-sans {
            font-family: 'Lato', sans-serif;
        }
        .form-section {
            page-break-inside: avoid;
        }
        @media print {
            .no-print {
                display: none !important;
            }
            body {
                font-size: 12pt;
            }
            .form-container {
                box-shadow: none;
                border: none;
            }
            body * {
                visibility: hidden;
            }
            .print-area, .print-area * {
                visibility: visible;
            }
            .print-area {
                position: absolute;
                left: 0;
                top: 0;
                width: 100%;
                color: black !important;
                background: white !important;
            }
            .print-area input, .print-area textarea {
                border: none;
                border-bottom: 1px solid black;
                background: white;
            }
        }
        .modal {
            display: none;
            position: fixed;
            z-index: 50;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            overflow: auto;
            background-color: rgba(0,0,0,0.4);
        }
        .modal-content {
            background-color: #fefefe;
            margin: 15% auto;
            padding: 20px;
            border: 1px solid #888;
            width: 80%;
            max-width: 500px;
            border-radius: 8px;
        }
        .close {
            color: #aaa;
            float: right;
            font-size: 28px;
            font-weight: bold;
        }
        .close:hover,
        .close:focus {
            color: black;
            text-decoration: none;
            cursor: pointer;
        }
    </style>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        purple: {
                            50: '#f9f8fc',
                            100: '#f3f1f9',
                            200: '#e9e3f4',
                            300: '#d9d0ed',
                            400: '#c7b8e3',
                            500: '#b39cd6',
                            600: '#9f81c9',
                            700: '#8a65b9',
                            800: '#744ba5',
                            900: '#5f368e',
                            950: '#48226d',
                        },
                        pink: {
                            50: '#fdf4f7',
                            100: '#fce8ef',
                            200: '#fad0df',
                            300: '#f7b2cb',
                            400: '#ffb6c1',
                            500: '#f47ca0',
                            600: '#e95f86',
                            700: '#dd436e',
                            800: '#c92c59',
                            900: '#a91f48',
                            950: '#870f37',
                        },
                        blue: {
                            50: '#f4f8fa',
                            100: '#e9f0f5',
                            200: '#d7e2ea',
                            300: '#c0d0de',
                            400: '#b0c4de',
                            500: '#92a8c9',
                            600: '#758cb3',
                            700: '#5c729d',
                            800: '#475a82',
                            900: '#35446a',
                            950: '#222c4a',
                        },
                        yellow: {
                            50: '#fffdf5',
                            100: '#fffbeb',
                            200: '#fff7d6',
                            300: '#fff2c1',
                            400: '#fffacd',
                            500: '#f5e9a3',
                            600: '#ebd97a',
                            700: '#e1c851',
                            800: '#d7b728',
                            900: '#cda600',
                            950: '#a38300',
                        }
                    }
                }
            }
        }
    </script>
</head>
<body class="font-sans text-purple-900 bg-white">
    <!-- Navigation -->
    <nav class="bg-white shadow-sm sticky top-0 z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-16">
                <div class="flex items-center">
                    <div class="flex-shrink-0 flex items-center">
                        <img src='https://i.postimg.cc/ncrCsgHY/tlc-logo.png' alt='tlc-logo' class="h-10 w-10">
                        <span class="ml-2 font-serif text-xl font-bold text-purple-700">TLC Family Services</span>
                    </div>
                </div>
                <div class="hidden md:ml-6 md:flex md:items-center md:space-x-8">
                    <a href="../#home" class="px-3 py-2 text-sm font-medium text-purple-900 border-b-2 border-transparent hover:border-purple-500">Home</a>
                    <a href="../#services" class="px-3 py-2 text-sm font-medium text-purple-900 border-b-2 border-transparent hover:border-purple-500">Services</a>
                    <a href="../#resources" class="px-3 py-2 text-sm font-medium text-purple-900 border-b-2 border-transparent hover:border-purple-500">Resources</a>
                    <a href="../#events" class="px-3 py-2 text-sm font-medium text-purple-900 border-b-2 border-transparent hover:border-purple-500">Events</a>
                    <a href="../#about" class="px-3 py-2 text-sm font-medium text-purple-900 border-b-2 border-transparent hover:border-purple-500">About Us</a>
                    <a href="#" onclick="openEmail()" class="inline-flex items-center px-4 py-2 border border-transparent text-sm font-medium rounded-md shadow-sm text-white bg-purple-600 hover:bg-purple-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-purple-500">
                        Contact Us
                    </a>
                </div>
                <div class="-mr-2 flex items-center md:hidden">
                    <button type="button" id="mobile-menu-button" class="inline-flex items-center justify-center p-2 rounded-md text-purple-400 hover:text-purple-500 hover:bg-purple-100 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-purple-500">
                        <span class="sr-only">Open main menu</span>
                        <i class="fas fa-bars"></i>
                    </button>
                </div>
            </div>
        </div>
        <!-- Mobile menu -->
        <div class="hidden md:hidden" id="mobile-menu">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3 bg-white">
                <a href="../#home" class="text-purple-900 hover:text-purple-700 block px-3 py-2 rounded-md text-base font-medium">Home</a>
                <a href="../#services" class="text-purple-900 hover:text-purple-700 block px-3 py-2 rounded-md text-base font-medium">Services</a>
                <a href="../#resources" class="text-purple-900 hover:text-purple-700 block px-3 py-2 rounded-md text-base font-medium">Resources</a>
                <a href="../#events" class="text-purple-900 hover:text-purple-700 block px-3 py-2 rounded-md text-base font-medium">Events</a>
                <a href="../#about" class="text-purple-900 hover:text-purple-700 block px-3 py-2 rounded-md text-base font-medium">About Us</a>
                <a href="#" onclick="openEmail()" class="bg-purple-600 hover:bg-purple-700 text-white block px-3 py-2 rounded-md text-base font-medium transition duration-300">Contact Us</a>
            </div>
        </div>
    </nav>

    <div class="container mx-auto px-4 py-8 max-w-4xl">
        <div class="bg-white rounded-lg shadow-md p-6 form-container">
            <div class="text-center mb-8">
                <h1 class="font-serif text-3xl font-bold text-purple-800">Additional Consent Forms</h1>
                <p class="text-pink-700 mt-2">Please fill out these forms completely and accurately</p>
            </div>

            <form id="additional-consent-form" action="https://formspree.io/f/mzzvjdow" method="POST" class="space-y-8">
                <input type="hidden" name="form_type" value="Additional Consent Forms">

                <!-- Consent of Participation -->
                <div class="form-section border-b pb-6">
                    <h2 class="font-serif text-xl font-bold text-purple-800 mb-4">Consent of Participation</h2>
                    <div class="space-y-4 text-pink-700">
                        <p>I, <input type="text" name="client_name_participation" class="border-b border-purple-300 focus:outline-none focus:border-purple-500 inline-block w-64" placeholder="Your Name">, agree to participate in mental health services (Individual, Group and Family Therapy) provided by TLC Family Services and will participate in the development of the Individual Treatment Plan for Mental Health services. I hereby give consent for services to be provided.</p>
                        <p>I have been informed and received copies of the Client Rights and Responsibilities and Discharge and Grievance Procedures by TLC Family Services.</p>
                    </div>
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-4 mt-6">
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Client/Parent/Guardian (please circle one)</label>
                            <select name="relationship_participation" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                                <option value="Client">Client</option>
                                <option value="Parent">Parent</option>
                                <option value="Guardian">Guardian</option>
                            </select>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Staff Signature</label>
                            <input type="text" name="staff_signature_participation" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="Type staff signature">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Date</label>
                            <input type="date" name="date_participation" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                    </div>
                </div>

                <!-- Practice Financial Agreement -->
                <div class="form-section border-b pb-6">
                    <h2 class="font-serif text-xl font-bold text-purple-800 mb-4">Practice Financial Agreement</h2>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4 text-pink-700">
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Client's Name</label>
                            <input type="text" name="client_name_financial" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Monthly Income</label>
                            <input type="text" name="monthly_income" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Source of Income</label>
                            <input type="text" name="source_income" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div class="flex items-center">
                            <label class="text-sm font-medium text-pink-700 mr-4">Does Member have MA?</label>
                            <div class="flex items-center">
                                <input type="radio" name="has_ma" value="Yes" class="mr-2">
                                <span>Yes</span>
                                <input type="radio" name="has_ma" value="No" class="ml-4 mr-2">
                                <span>No</span>
                            </div>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">If Yes, MA #</label>
                            <input type="text" name="ma_number" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">If other insurance, name of company</label>
                            <input type="text" name="insurance_company" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Policy Number</label>
                            <input type="text" name="policy_number" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div class="flex items-center">
                            <label class="text-sm font-medium text-pink-700 mr-4">Will member be billed?</label>
                            <div class="flex items-center">
                                <input type="radio" name="will_be_billed" value="Yes" class="mr-2">
                                <span>Yes</span>
                                <input type="radio" name="will_be_billed" value="No" class="ml-4 mr-2">
                                <span>No</span>
                            </div>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">If Yes, amount of charge per day: $</label>
                            <input type="text" name="charge_amount" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                    </div>
                    <p class="text-pink-700 mt-4">TLC Family Services has explained the Health Care Services policy. I understand that if I do not have insurance coverage, I may be billed by TLC Family Services for receiving any of the services provided by TLC Family Services.</p>
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-4 mt-6">
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Client Signature</label>
                            <input type="text" name="client_signature_financial" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="Type your signature">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Date</label>
                            <input type="date" name="date_financial" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Staff Signature</label>
                            <input type="text" name="staff_signature_financial" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="Type staff signature">
                        </div>
                    </div>
                </div>

                <!-- Advanced Mental Health Directives -->
                <div class="form-section border-b pb-6">
                    <h2 class="font-serif text-xl font-bold text-purple-800 mb-4">Advanced Mental Health Directives</h2>
                    <p class="text-pink-700">(Applicable if Age 16 or Older)</p>
                    <p class="text-pink-700 mt-4">I, <input type="text" name="client_name_directives" class="border-b border-purple-300 focus:outline-none focus:border-purple-500 inline-block w-64" placeholder="Your Name">, have received information regarding Advanced Mental Health Directives.</p>
                    <div class="mt-4">
                        <p class="text-pink-700 mb-2">Please Check One:</p>
                        <div class="flex items-center mb-2">
                            <input type="radio" name="directives_status" value="Has Directive" class="mr-2">
                            <label class="text-pink-700">I currently have an Advanced Mental Health Directive and have given TLC Family Services a copy.</label>
                        </div>
                        <div class="flex items-center">
                            <input type="radio" name="directives_status" value="No Directive" class="mr-2">
                            <label class="text-pink-700">I do not currently have an Advanced Mental Health Directive</label>
                        </div>
                    </div>
                    <p class="text-pink-700 font-semibold mt-4">IF YOU DO NOT HAVE AN ADVANCED MENTAL HEALTH DIRECTIVE AND WOULD LIKE ONE, PLEASE HAVE YOUR THERAPIST TO ASSIST YOU IN MAKING AN ADVANCED MENTAL HEALTH DIRECTIVE.</p>
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-4 mt-6">
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Client (Age 16 or older) / Parent / Guardian</label>
                            <select name="relationship_directives" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                                <option value="Client">Client (Age 16 or older)</option>
                                <option value="Parent">Parent</option>
                                <option value="Guardian">Guardian</option>
                            </select>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Staff Signature</label>
                            <input type="text" name="staff_signature_directives" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="Type staff signature">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Date</label>
                            <input type="date" name="date_directives" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                    </div>
                </div>

                <!-- Emergency Information -->
                <div class="form-section border-b pb-6">
                    <h2 class="font-serif text-xl font-bold text-purple-800 mb-4">Emergency Information</h2>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4 text-pink-700">
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Patient's Name</label>
                            <input type="text" name="patient_name_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">DOB</label>
                            <input type="date" name="dob_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div class="md:col-span-2">
                            <label class="block text-sm font-medium text-pink-700">Address</label>
                            <div class="grid grid-cols-3 gap-2">
                                <input type="text" name="street_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="Street">
                                <input type="text" name="city_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="City">
                                <input type="text" name="state_zip_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="State Zip">
                            </div>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Phone</label>
                            <input type="tel" name="phone_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Business Telephone</label>
                            <input type="tel" name="business_phone_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div class="md:col-span-2">
                            <label class="block text-sm font-medium text-pink-700">Medical Assistance No/MCO if applicable</label>
                            <input type="text" name="medical_assistance_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Parent(s)/Guardian(s) Name</label>
                            <input type="text" name="parent_guardian_name_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div class="md:col-span-2">
                            <label class="block text-sm font-medium text-pink-700">Address</label>
                            <div class="grid grid-cols-3 gap-2">
                                <input type="text" name="parent_street_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="Street">
                                <input type="text" name="parent_city_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="City">
                                <input type="text" name="parent_state_zip_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="State Zip">
                            </div>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Primary Physician</label>
                            <input type="text" name="primary_physician_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div class="md:col-span-2">
                            <label class="block text-sm font-medium text-pink-700">Address</label>
                            <div class="grid grid-cols-3 gap-2">
                                <input type="text" name="physician_street_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="Street">
                                <input type="text" name="physician_city_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="City">
                                <input type="text" name="physician_state_zip_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="State Zip">
                            </div>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Phone</label>
                            <input type="tel" name="physician_phone_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Fax</label>
                            <input type="text" name="physician_fax_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div class="md:col-span-2">
                            <label class="block text-sm font-medium text-pink-700">Allergies</label>
                            <input type="text" name="allergies_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div class="md:col-span-2">
                            <label class="block text-sm font-medium text-pink-700">Somatic Health Problems</label>
                            <input type="text" name="somatic_problems_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Case Manager (if Applicable)</label>
                            <input type="text" name="case_manager_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div class="md:col-span-2">
                            <label class="block text-sm font-medium text-pink-700">Address</label>
                            <input type="text" name="case_manager_address_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Phone</label>
                            <input type="tel" name="case_manager_phone_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Fax</label>
                            <input type="text" name="case_manager_fax_emergency" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                    </div>
                    <p class="text-pink-700 font-semibold mt-4">Listed below are people who can be contacted in case of an emergency.</p>
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-4 mt-4">
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Name</label>
                            <input type="text" name="emergency_contact1_name" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                            <label class="block text-sm font-medium text-pink-700 mt-2">Daytime Phone</label>
                            <input type="tel" name="emergency_contact1_phone" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                            <label class="block text-sm font-medium text-pink-700 mt-2">Address</label>
                            <input type="text" name="emergency_contact1_address" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Name</label>
                            <input type="text" name="emergency_contact2_name" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                            <label class="block text-sm font-medium text-pink-700 mt-2">Daytime Phone</label>
                            <input type="tel" name="emergency_contact2_phone" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                            <label class="block text-sm font-medium text-pink-700 mt-2">Address</label>
                            <input type="text" name="emergency_contact2_address" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Name</label>
                            <input type="text" name="emergency_contact3_name" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                            <label class="block text-sm font-medium text-pink-700 mt-2">Daytime Phone</label>
                            <input type="tel" name="emergency_contact3_phone" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                            <label class="block text-sm font-medium text-pink-700 mt-2">Address</label>
                            <input type="text" name="emergency_contact3_address" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                    </div>
                    <p class="text-pink-700 text-sm mt-2">** If patient is a child, will need third emergency contact filled out on form.</p>
                </div>

                <!-- Medical Evaluation Form -->
                <div class="form-section border-b pb-6">
                    <h2 class="font-serif text-xl font-bold text-purple-800 mb-4">Medical Evaluation Form</h2>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4 text-pink-700">
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Patient's Name</label>
                            <input type="text" name="patient_name_medical" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Date</label>
                            <input type="date" name="date_medical" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                    </div>
                    <p class="text-pink-700 mt-4">Please check if you have experienced any of the following: (explain below)</p>
                    <div class="grid grid-cols-2 md:grid-cols-3 gap-2 mt-2">
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Asthma" class="mr-2">
                            <label class="text-pink-700">Asthma</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Abdominal pains" class="mr-2">
                            <label class="text-pink-700">Abdominal pains</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Allergies/other than meds" class="mr-2">
                            <label class="text-pink-700">Allergies/other than meds</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Bedwetting" class="mr-2">
                            <label class="text-pink-700">Bedwetting</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Blackouts" class="mr-2">
                            <label class="text-pink-700">Blackouts</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Blood pressure problems" class="mr-2">
                            <label class="text-pink-700">Blood pressure problems</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Blurred vision" class="mr-2">
                            <label class="text-pink-700">Blurred vision</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Cancer" class="mr-2">
                            <label class="text-pink-700">Cancer</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Convulsions" class="mr-2">
                            <label class="text-pink-700">Convulsions</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Diabetes" class="mr-2">
                            <label class="text-pink-700">Diabetes</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Dietary problems" class="mr-2">
                            <label class="text-pink-700">Dietary problems</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Dizziness" class="mr-2">
                            <label class="text-pink-700">Dizziness</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Fainting spells" class="mr-2">
                            <label class="text-pink-700">Fainting spells</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Frequent illness" class="mr-2">
                            <label class="text-pink-700">Frequent illness</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Head injuries" class="mr-2">
                            <label class="text-pink-700">Head injuries</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Headaches" class="mr-2">
                            <label class="text-pink-700">Headaches</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Heart problems" class="mr-2">
                            <label class="text-pink-700">Heart problems</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="High Fever" class="mr-2">
                            <label class="text-pink-700">High Fever</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Hysterical attacks" class="mr-2">
                            <label class="text-pink-700">Hysterical attacks</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Incoordination" class="mr-2">
                            <label class="text-pink-700">Incoordination</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Injuries/accidents" class="mr-2">
                            <label class="text-pink-700">Injuries/accidents</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Insomnia" class="mr-2">
                            <label class="text-pink-700">Insomnia</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Kidney problems" class="mr-2">
                            <label class="text-pink-700">Kidney problems</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Loss of consciousness" class="mr-2">
                            <label class="text-pink-700">Loss of consciousness</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Menstrual problems" class="mr-2">
                            <label class="text-pink-700">Menstrual problems</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Muscular/skeletal abnor." class="mr-2">
                            <label class="text-pink-700">Muscular/skeletal abnor.</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Nausea" class="mr-2">
                            <label class="text-pink-700">Nausea</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Nightmares" class="mr-2">
                            <label class="text-pink-700">Nightmares</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Nosebleeds" class="mr-2">
                            <label class="text-pink-700">Nosebleeds</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Paralysis, Numbness, Weakness" class="mr-2">
                            <label class="text-pink-700">Paralysis, Numbness, Weakness</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Peptic Ulcer" class="mr-2">
                            <label class="text-pink-700">Peptic Ulcer</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Ringing in ears" class="mr-2">
                            <label class="text-pink-700">Ringing in ears</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Serious illness" class="mr-2">
                            <label class="text-pink-700">Serious illness</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Sexual Problems" class="mr-2">
                            <label class="text-pink-700">Sexual Problems</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Sleepwalking" class="mr-2">
                            <label class="text-pink-700">Sleepwalking</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Strange odor" class="mr-2">
                            <label class="text-pink-700">Strange odor</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Thyroid" class="mr-2">
                            <label class="text-pink-700">Thyroid</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Unexplained crying" class="mr-2">
                            <label class="text-pink-700">Unexplained crying</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Weight problems" class="mr-2">
                            <label class="text-pink-700">Weight problems</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="medical_conditions[]" value="Other" class="mr-2">
                            <label class="text-pink-700">Other (explain)</label>
                        </div>
                    </div>
                    <label class="block text-sm font-medium text-pink-700 mt-4">Explanation</label>
                    <textarea name="medical_explanation" rows="4" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500"></textarea>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4 mt-4">
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Allergic to</label>
                            <input type="text" name="allergic_to" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Medications</label>
                            <input type="text" name="medications_medical" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Immunizations</label>
                            <input type="text" name="immunizations" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Current</label>
                            <input type="text" name="current_medical" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div class="md:col-span-2">
                            <label class="block text-sm font-medium text-pink-700">Other recommendations</label>
                            <input type="text" name="other_recommendations" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                    </div>
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-4 mt-6">
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Client/Parent/Guardian Signature</label>
                            <input type="text" name="client_signature_medical" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="Type your signature">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Date</label>
                            <input type="date" name="date_medical" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Staff Signature</label>
                            <input type="text" name="staff_signature_medical" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="Type staff signature">
                        </div>
                    </div>
                </div>

                <!-- Risk Management Plan -->
                <div class="form-section border-b pb-6">
                    <h2 class="font-serif text-xl font-bold text-purple-800 mb-4">Risk Management Plan</h2>
                    <div class="space-y-4 text-pink-700">
                        <p>It is the policy of TLC Family Services to provide safe, effective, and efficient services, to the extent possible, through adherence to risk identification and management procedures.</p>
                        <p class="font-semibold">PURPOSE:</p>
                        <p>The purpose of the Risk Management policy is to ensure:</p>
                        <ol class="list-decimal pl-5 space-y-2">
                            <li>TLC Family Services is aware of all its current risks and allocates resources in an appropriate manner to manage its risks.</li>
                            <li>Whenever possible, the risk of injury, damage of loss of persons served, staff, or the organizations is removed, and where not, is managed in a way that minimizes the risk.</li>
                            <li>Staff understands and uses these procedures for risk identification, assessment, reporting and management.</li>
                            <li>TLC Family Services meets its statutory requirements to comply with current Federal and State Health and safety laws and requirements.</li>
                            <li>TLC Family Services complies with the relevant standards in accordance with regulations.</li>
                        </ol>
                        <p class="font-semibold">GENERAL INFORMATION:</p>
                        <p class="font-semibold">Individual Members of Staff:</p>
                        <p>It is the responsibility of the licensed therapist to be alert to risk and it is their duty to report them through their chain of command so that appropriate action can be taken to assess report and manage the risks.</p>
                        <p class="font-semibold">Licensed Therapist Responsibilities:</p>
                        <p>They are responsible for strategic risk management; for overall day to day risk management; and for day to day client crisis and risk management; to ensure effective risk management is taking place within the program; to be alert to risks and report them through the line of management so the appropriate action takes place.</p>
                    </div>
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-4 mt-6">
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Client/Parent/Guardian's Signature</label>
                            <input type="text" name="client_signature_risk" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="Type your signature">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Staff Signature</label>
                            <input type="text" name="staff_signature_risk" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="Type staff signature">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Date</label>
                            <input type="date" name="date_risk" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                    </div>
                </div>

                <!-- Crisis Management Plan -->
                <div class="form-section border-b pb-6">
                    <h2 class="font-serif text-xl font-bold text-purple-800 mb-4">Crisis Management Plan</h2>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4 text-pink-700">
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Client's Name</label>
                            <input type="text" name="client_name_crisis" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                    </div>
                    <p class="text-pink-700 mt-4">Crisis is a sudden change in the client's behavior in response to stress or other painful feelings. It is often negative due to the client's lack of experience or inability to cope with personal or interpersonal problems. The goals of crisis management are to: provide immediate emotional support and reduce stress, decrease the risk of harm to the client or others and teach better, more constructive ways for dealing with stress or other painful feelings.</p>
                    <p class="text-pink-700 font-semibold mt-4">Our Privacy Practices:</p>
                    <p class="text-pink-700">Our practice promises to maintain the confidentiality of your protected health information (PHI). PHI is health information about you that we have in our records. We will not share this information, in whole or in part, with any person or entity without your consent. In addition, we commit to delivering our services in a manner that maintains confidentiality. We will coordinate services with primary care physicians, referring agencies, schools or other stakeholders with your written consent.</p>
                    <p class="text-pink-700 mt-4">Part of good crisis management is knowing what to expect. Generally, a person's response to stress or negative situations is the same. With that in mind, check the responses that relate to your client.</p>
                    <p class="text-pink-700 font-semibold mt-4">When my client is upset, he/she: (please check all that applies)</p>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-2 mt-2">
                        <div class="flex items-center">
                            <input type="checkbox" name="crisis_responses[]" value="Uses profanity" class="mr-2">
                            <label class="text-pink-700">Uses profanity (i.e.: cursing, swearing, and vulgar language)</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="crisis_responses[]" value="Makes verbal or physical threats" class="mr-2">
                            <label class="text-pink-700">Makes verbal or physical threats (i.e.: violating personal space)</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="crisis_responses[]" value="Has a rage reaction" class="mr-2">
                            <label class="text-pink-700">Has a rage reaction (i.e.: temper tantrum, screaming, door slamming)</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="crisis_responses[]" value="Challenges authority" class="mr-2">
                            <label class="text-pink-700">Challenges authority (i.e.: talks back to parents, teachers, police, etc.)</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="crisis_responses[]" value="Tries to hurt others" class="mr-2">
                            <label class="text-pink-700">Tries to hurt others (i.e.: hits, kicks, bites, spits, pushes, etc.)</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="crisis_responses[]" value="Tries to hurt himself/herself" class="mr-2">
                            <label class="text-pink-700">Tries to hurt himself/herself</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="crisis_responses[]" value="Destroys property" class="mr-2">
                            <label class="text-pink-700">Destroys property</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="crisis_responses[]" value="Runs away" class="mr-2">
                            <label class="text-pink-700">Runs away</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="crisis_responses[]" value="Ignores rules or directions" class="mr-2">
                            <label class="text-pink-700">Ignores rules or directions</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="crisis_responses[]" value="Makes bad decisions" class="mr-2">
                            <label class="text-pink-700">Makes bad decisions</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="crisis_responses[]" value="Uses drugs or alcohol" class="mr-2">
                            <label class="text-pink-700">Uses drugs or alcohol</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="crisis_responses[]" value="Seeks out weapons or other harmful objects" class="mr-2">
                            <label class="text-pink-700">Seeks out weapons or other harmful objects</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="crisis_responses[]" value="Ignores everybody" class="mr-2">
                            <label class="text-pink-700">Refuses to talk to anybody</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="crisis_responses[]" value="Will only talk to" class="mr-2">
                            <label class="text-pink-700">Will only talk to <input type="text" name="talk_to_person" class="border-b border-purple-300 focus:outline-none focus:border-purple-500 inline-block w-32"></label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="crisis_responses[]" value="Targets or starts fights" class="mr-2">
                            <label class="text-pink-700">Targets or starts fights or arguments with others</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="crisis_responses[]" value="Demands to be left alone" class="mr-2">
                            <label class="text-pink-700">Demands to be left alone</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="crisis_responses[]" value="Makes homicidal threats" class="mr-2">
                            <label class="text-pink-700">Makes homicidal threats ("I'm going to kill...")</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="crisis_responses[]" value="Makes suicidal threats" class="mr-2">
                            <label class="text-pink-700">Makes suicidal threats ("I'm going to kill myself.")</label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="crisis_responses[]" value="Acts out by 1" class="mr-2">
                            <label class="text-pink-700">Acts out by <input type="text" name="acts_out_1" class="border-b border-purple-300 focus:outline-none focus:border-purple-500 inline-block w-32"></label>
                        </div>
                        <div class="flex items-center">
                            <input type="checkbox" name="crisis_responses[]" value="Acts out by 2" class="mr-2">
                            <label class="text-pink-700">Acts out by <input type="text" name="acts_out_2" class="border-b border-purple-300 focus:outline-none focus:border-purple-500 inline-block w-32"></label>
                        </div>
                    </div>
                    <p class="text-pink-700 font-semibold mt-4">TIPS FOR MANAGING A CLIENT IN CRISIS:</p>
                    <ol class="list-decimal pl-5 space-y-2 text-pink-700">
                        <li>Control the space where the client is acting out. Make sure that there are no objects around that could be used as weapons. Prevent the client from being able to harm himself/herself or others.</li>
                        <li>Acknowledge the client's feelings and give him/her time and space to vent. Allow him/her to talk without being interrupted. Avoid discussion or interaction until he/she is calmer.</li>
                        <li>Don't take it personal! Ignore negative comments directed towards you; your response will often make the client act out more.</li>
                        <li>Look for chances to reinforce good decisions. If the client has stopped throwing things, say, "I'm glad you stopped throwing things." If he/she has stopped using profanity, acknowledge that they are communicating more appropriately.</li>
                        <li>Get a feel for when the client is ready to hear you. Speak calmly and assertively...but don't be bossy or judgmental.</li>
                        <li>Present the client with your expectation(s) and offer to help. For example, "You know you're going to have to clean that up; do you want me to get the broom?"</li>
                        <li>When the client is calmer, take time immediately to review what just happened and discuss better ways that the client could deal with the situation "next time".</li>
                    </ol>
                    <p class="text-pink-700 mt-4">There will be a "next time"; so reinforce the new plan and let the client know that you will be looking to see him/her put the new plan into action.</p>
                    <p class="text-pink-700 mt-4">If the CLIENT should exhibit behaviors that pose harm to his/herself or others, staff will:</p>
                    <ul class="list-disc pl-5 space-y-1 text-pink-700">
                        <li>Limit client's access to weapons or items that can be used as weapons;</li>
                        <li>Remove the person(s) who is/are the current target;</li>
                        <li>Offer the client options and set limits;</li>
                        <li>Use verbal interventions and proximity control to help the client deescalate, and;</li>
                        <li>Assist the client with reintegration.</li>
                    </ul>
                    <p class="text-pink-700 mt-4">Should unsafe behavior(s) persist, staff will:</p>
                    <ul class="list-disc pl-5 space-y-1 text-pink-700">
                        <li>Contact Center Director at 667-355-2334 (during business hours)</li>
                        <li>Contact our after-hours crisis number at 667-355-2334</li>
                        <li>Contact 911</li>
                        <li>Transport or refer client to closest Emergency Room</li>
                    </ul>
                    <label class="block text-sm font-medium text-pink-700 mt-4">Other specific crisis management/safety precautions determined by specific situation:</label>
                    <textarea name="other_crisis_precautions" rows="4" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500"></textarea>
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-4 mt-6">
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Client/Parent/Guardian's Signature</label>
                            <input type="text" name="client_signature_crisis" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="Type your signature">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Staff Signature</label>
                            <input type="text" name="staff_signature_crisis" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="Type staff signature">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Date</label>
                            <input type="date" name="date_crisis" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                    </div>
                </div>

                <!-- Grievances Procedure -->
                <div class="form-section border-b pb-6">
                    <h2 class="font-serif text-xl font-bold text-purple-800 mb-4">Grievances Procedure</h2>
                    <p class="text-pink-700">Clients receiving mental health services at TLC Family Services can follow this procedure to file grievances:</p>
                    <p class="text-pink-700 font-semibold mt-4">Step 1:</p>
                    <p class="text-pink-700">Begin by expressing your concern to your program counselor. If this does not satisfy you, ask for a Client Grievance Form and submit the form to the Rehabilitation specialist or Program Director. If you need assistance completing this form or you have difficulty in reading the instructions, you are entitled to have a confidential conference with the Rehabilitation Specialist to explain the policy. Your complaint or grievance will be heard within three (3) working days.</p>
                    <p class="text-pink-700 italic">You may skip any of these steps at any time.</p>
                    <p class="text-pink-700 font-semibold mt-4">Step 2:</p>
                    <p class="text-pink-700">If you feel your grievance has not been resolved, submit the Client Grievance Form to the Grievance Committee through the Office Manager. The Committee is comprised of the Rehabilitation Specialist, Program Director, and PRP Coordinator. If you cannot read or write, you are entitled to receive assistance from the Rehabilitation Specialist.</p>
                    <p class="text-pink-700 italic">You may skip any of these steps at any time.</p>
                    <p class="text-pink-700 font-semibold mt-4">Step 3:</p>
                    <p class="text-pink-700">You may also directly request for an appointment with the Program Director through the Office Manager. The Office Manager will ensure your appointment is scheduled within five (5) working days.</p>
                    <p class="text-pink-700 italic">You may skip any of these steps at any time.</p>
                    <p class="text-pink-700 font-semibold mt-4">Step 4:</p>
                    <p class="text-pink-700">If you feel your grievance has not been satisfactorily resolved, you may directly approach the Core Service Agency for your locality.</p>
                    <ul class="list-disc pl-5 space-y-1 text-pink-700">
                        <li>Baltimore City (410) 834-2647</li>
                        <li>Baltimore County (410) 887-4859</li>
                        <li>Harford County (410) 803-8726</li>
                        <li>Cecil County (410) 996-5112</li>
                    </ul>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4 mt-6">
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Signature</label>
                            <input type="text" name="signature_grievance" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="Type your signature">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Date</label>
                            <input type="date" name="date_grievance" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                    </div>
                </div>

                <!-- Client Consent to Release Information -->
                <div class="form-section border-b pb-6">
                    <h2 class="font-serif text-xl font-bold text-purple-800 mb-4">Client Consent to Release Information</h2>
                    <p class="text-pink-700 font-semibold">CLIENT INFORMATION:</p>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4 mt-4 text-pink-700">
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Last Name</label>
                            <input type="text" name="last_name_release" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">First Name</label>
                            <input type="text" name="first_name_release" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">MI</label>
                            <input type="text" name="mi_release" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div class="flex items-center">
                            <label class="text-sm font-medium text-pink-700 mr-4">Gender</label>
                            <div class="flex items-center">
                                <input type="radio" name="gender_release" value="M" class="mr-2">
                                <span>M</span>
                                <input type="radio" name="gender_release" value="F" class="ml-4 mr-2">
                                <span>F</span>
                            </div>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">DOB</label>
                            <input type="date" name="dob_release" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">SS#</label>
                            <input type="text" name="ssn_release" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Race</label>
                            <input type="text" name="race_release" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Address</label>
                            <input type="text" name="address_release" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Tel (Mobile)</label>
                            <input type="tel" name="mobile_release" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Tel (Home)</label>
                            <input type="tel" name="home_phone_release" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                    </div>
                    <p class="text-pink-700 font-semibold mt-4">Provider Name:</p>
                    <p class="text-pink-700">Licensed Professional</p>
                    <p class="text-pink-700 font-semibold mt-4">Organization Address:</p>
                    <p class="text-pink-700">TLC Family Services</p>
                    <p class="text-pink-700">Phone #: 667-355-2334</p>
                    <p class="text-pink-700 mt-4">I hereby authorize the licensed professional as my treatment provider to consult with other health care professionals as necessary to ensure the appropriateness of my care. I also understand that the licensed professional will coordinate this care with my primary caretaker. I have read the client list of rights and responsibilities or had them read to me.</p>
                    <p class="text-pink-700 mt-4">This consent will remain in effect until the time I revoke this it in writing or word, or until one year after my last signature.</p>
                    <label class="block text-sm font-medium text-pink-700 mt-4">VALID UNTIL</label>
                    <input type="date" name="valid_until_release" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                    <p class="text-pink-700 italic mt-4">If signing for a minor child, I hereby affirm that I am the parent or legal guardian.</p>
                    <p class="text-pink-700 mt-4">Permission to release information to facilitate coordination of my care is hereby:</p>
                    <div class="flex items-center mt-2">
                        <div class="flex items-center mr-4">
                            <input type="radio" name="permission_release" value="Authorized" class="mr-2">
                            <label class="text-pink-700">Authorized</label>
                        </div>
                        <div class="flex items-center">
                            <input type="radio" name="permission_release" value="Withheld" class="mr-2">
                            <label class="text-pink-700">Withheld</label>
                        </div>
                    </div>
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-4 mt-6">
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Client Signature (or Guardian for minor)</label>
                            <input type="text" name="client_signature_release" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="Type your signature">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Witness Signature</label>
                            <input type="text" name="witness_signature_release" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="Type witness signature">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Date</label>
                            <input type="date" name="date_release" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                    </div>
                </div>

                <!-- Teletherapy Informed Consent Form -->
                <div class="form-section border-b pb-6">
                    <h2 class="font-serif text-xl font-bold text-purple-800 mb-4">Teletherapy Informed Consent Form</h2>
                    <p class="text-pink-700 font-semibold">CLIENT INFORMATION:</p>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4 mt-4 text-pink-700">
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Last Name</label>
                            <input type="text" name="last_name_teletherapy" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">First Name</label>
                            <input type="text" name="first_name_teletherapy" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">MI</label>
                            <input type="text" name="mi_teletherapy" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div class="flex items-center">
                            <label class="text-sm font-medium text-pink-700 mr-4">Gender</label>
                            <div class="flex items-center">
                                <input type="radio" name="gender_teletherapy" value="M" class="mr-2">
                                <span>M</span>
                                <input type="radio" name="gender_teletherapy" value="F" class="ml-4 mr-2">
                                <span>F</span>
                            </div>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">DOB</label>
                            <input type="date" name="dob_teletherapy" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">SS#</label>
                            <input type="text" name="ssn_teletherapy" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Race</label>
                            <input type="text" name="race_teletherapy" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Address</label>
                            <input type="text" name="address_teletherapy" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Tel (Mobile)</label>
                            <input type="tel" name="mobile_teletherapy" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Tel (Home)</label>
                            <input type="tel" name="home_phone_teletherapy" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                    </div>
                    <p class="text-pink-700 font-semibold mt-4">Provider Name:</p>
                    <p class="text-pink-700">Licensed Professional</p>
                    <p class="text-pink-700 font-semibold mt-4">Address:</p>
                    <p class="text-pink-700">TLC Family Services</p>
                    <p class="text-pink-700">Phone #: 667-355-2334</p>
                    <p class="text-pink-700 mt-4">I hereby consent to engage in teletherapy with the licensed professional. I understand that "teletherapy" includes holding therapy sessions via telephone/video conversations and education using interactive audio, video, or data communications. I understand that teletherapy also involves the oral and visual communication of my mental health information. I understand that I have the following rights with respect to teletherapy:</p>
                    <ol class="list-decimal pl-5 space-y-2 text-pink-700">
                        <li>The right to withhold or withdraw consent at any time without affecting my right to future care or treatment.</li>
                        <li>The laws that protect the confidentiality of my mental health information also apply to teletherapy. As such, I understand that the information disclosed by me during the course of my therapy is generally confidential. However, there are both mandatory and permissive exceptions to confidentiality, which are discussed in detail in other consent forms I have signed.</li>
                        <li>I understand that there are risks and consequences from teletherapy, including, but not limited to, the possibility, despite reasonable efforts on the part of the licensed professional that: the transmission of my information could be disrupted or distorted by technical failures; the transmission of my information could be interrupted by unauthorized persons; and/or the electronic storage of my mental health information could be accessed by unauthorized persons.</li>
                        <li>Teletherapy-based services may not be as complete as face-to-face services. I also understand that if the licensed professional believes I would be better served by another form of therapeutic services (e.g. face-to-face services), I will be referred to a professional who can provide such services in my area.</li>
                        <li>I understand that there are potential risks and benefits associated with any form of psychotherapy, and that despite my efforts and the efforts of my therapist, my condition may not improve, and in some cases may even get worse.</li>
                        <li>I understand that although I may benefit from teletherapy, the results cannot guaranteed or assured.</li>
                        <li>I accept that teletherapy does not provide emergency services. During our first session, the licensed professional and I will discuss an emergency response plan. If I am, therefore, experiencing an emergency situation, I understand that I can call 911 or proceed to the nearest hospital emergency room for help. If I am having suicidal thoughts or making plans to harm myself, I can call the National Suicide Prevention Lifeline at 1.800.273 TALK (8255) for free 24-hour hotline support.</li>
                        <li>I understand that the licensed professional shall be responsible for (1) providing the necessary computer, and internet access for my video therapy sessions; (2) the information security on the computer; and (3) arranging a location with sufficient lighting and privacy that shall be free from distractions or intrusions for my video therapy sessions for my video therapy sessions.</li>
                        <li>I have read, understood, and have agreed to the information provided above. This consent will remain in effect until the time I revoke it in writing or word, or until one year after my last signature.</li>
                    </ol>
                    <label class="block text-sm font-medium text-pink-700 mt-4">VALID UNTIL</label>
                    <input type="date" name="valid_until_teletherapy" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                    <p class="text-pink-700 italic mt-4">If signing for a minor child, I hereby affirm that I am the parent or legal guardian.</p>
                    <p class="text-pink-700 mt-4">Permission for teletherapy-based services to facilitate therapy sessions is hereby:</p>
                    <div class="flex items-center mt-2">
                        <div class="flex items-center mr-4">
                            <input type="radio" name="permission_teletherapy" value="Authorized" class="mr-2">
                            <label class="text-pink-700">Authorized</label>
                        </div>
                        <div class="flex items-center">
                            <input type="radio" name="permission_teletherapy" value="Withheld" class="mr-2">
                            <label class="text-pink-700">Withheld</label>
                        </div>
                    </div>
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-4 mt-6">
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Client Signature (or Guardian for minor)</label>
                            <input type="text" name="client_signature_teletherapy" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="Type your signature">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Witness Signature</label>
                            <input type="text" name="witness_signature_teletherapy" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="Type witness signature">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Date</label>
                            <input type="date" name="date_teletherapy" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                    </div>
                </div>

                <!-- Confidentiality & Privacy Practices Disclosure Statement -->
                <div class="form-section">
                    <h2 class="font-serif text-xl font-bold text-purple-800 mb-4">Confidentiality & Privacy Practices Disclosure Statement</h2>
                    <div class="space-y-4 text-pink-700">
                        <p>With few exceptions, our conversations are confidential. State law, federal regulations and our code of ethics specifically guarantee this confidentiality. There are some situations, however, in which confidentiality cannot be guaranteed. They fall within the following categories:</p>
                        <ul class="list-disc pl-5 space-y-1">
                            <li>We must notify appropriate persons if we feel you may harm another individual.</li>
                            <li>We must report any occurrence of child abuse (past or present), or the abuse, neglect or exploitation of the elderly.</li>
                            <li>We will have to respond to a subpoena accompanied by a court order.</li>
                            <li>We will have to respond to any situation in which we believe you may harm yourself.</li>
                        </ul>
                        <p class="font-semibold">Our Privacy Practices:</p>
                        <p>TLC Family Services promises to maintain the confidentiality of your protected health information (PHI). PHI is health information about you that we have in our records. We will not share this information, in whole or in part, with any person or entity without your consent. In addition, we commit to delivering our services in a manner that maintains confidentiality. We will coordinate services with primary care physicians, referring agencies, schools or other stakeholders with your written consent.</p>
                        <p class="font-semibold">Federal & State Laws:</p>
                        <p>We are required by federal regulations called the "HIPAA Privacy Regulations" to protect the confidentiality of your health information. We are also required to comply with state laws that are often more stringent than the federal regulations. This, in essence, gives you double protection.</p>
                        <p class="font-semibold">Authorization to Disclose PHI:</p>
                        <p>It is our practice to obtain your authorization or consent before we disclose your PHI to another person or entity. You may revoke your authorization or consent at any time and for any reason.</p>
                        <p class="font-semibold">How We Use Your Protected Health Information:</p>
                        <p>We use your PHI solely for treatment, payment and health care operations. For example, we may use your PHI to plan and provide your care and treatment; communicate with health care professionals; obtain payment for our services; educate and train our staff; and assess and improve our services. We are also permitted to use or disclose your health information if required by law.</p>
                        <p class="font-semibold">Your Rights:</p>
                        <p>You have a right to request a restriction on certain uses and disclosures of your PHI; inspect and copy your PHI; request amendments to your PHI; and obtain an accounting or list of disclosures of your PHI. This access does not include records from outside agencies, such as hospitals, DOE etc. Such access to the file must be authorized by the Program Director, with a rotation of date and time entered in the file. If it is felt that, it would not be in the best interest of the member to access the file, a written summary of the file contents will be provided to the individual. A staff member must be present while the record is being reviewed by the member to ensure that nothing is removed or changed within the file contents. A member who disagrees with the contents of his/her records will have the opportunity to submit corrections/amendments, which would be included in the records.</p>
                        <p class="font-semibold">Our Duty:</p>
                        <p>It is our duty to provide you with a copy of this disclosure statement for your personal records at the point of intake. A duplicate can be provided for you at any time upon request.</p>
                        <p class="font-semibold">For More Information or to Report a Problem:</p>
                        <p>If you have questions or concerns regarding our privacy practices, feel free to contact TLC Family Services at 667-355-2334.</p>
                        <p class="font-semibold">Acknowledgement:</p>
                        <p>Please sign below to indicate that you have received a copy of the Confidentiality & Privacy Practices Disclosure Statement.</p>
                    </div>
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-4 mt-6">
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Client/Parent/Guardian's Signature</label>
                            <input type="text" name="client_signature_confidentiality" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="Type your signature">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Date</label>
                            <input type="date" name="date_confidentiality" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-pink-700">Staff Signature</label>
                            <input type="text" name="staff_signature_confidentiality" class="mt-1 block w-full border border-purple-300 rounded-md shadow-sm py-2 px-3 focus:outline-none focus:ring-purple-500 focus:border-purple-500" placeholder="Type staff signature">
                        </div>
                    </div>
                </div>

                <div class="flex space-x-4">
                    <button type="submit" class="flex-1 bg-purple-600 hover:bg-purple-700 text-white font-medium py-3 px-4 rounded-lg transition duration-300">Submit Acknowledgment</button>
                    <button type="button" onclick="printForm(document.body)" class="flex-1 bg-pink-500 hover:bg-pink-600 text-white font-medium py-3 px-4 rounded-lg transition duration-300">Print Copy</button>
                </div>
                <p id="status_additional" class="mt-4 text-sm text-pink-600 text-center"></p>
            </form>
        </div>
    </div>

    <!-- Footer -->
    <footer class="bg-purple-900 text-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
            <div class="grid md:grid-cols-4 gap-8">
                <div>
                    <div class="flex items-center">
                        <img src='https://i.postimg.cc/ncrCsgHY/tlc-logo.png' alt='tlc-logo' class="h-8 w-8">
                        <span class="ml-2 font-serif text-xl font-bold text-purple-300">TLC Family Services</span>
                    </div>
                    <p class="mt-4 text-purple-300 text-sm">
                        Growth Through Gentle Strength
                    </p>
                </div>
              
                <div>
                    <h3 class="font-serif text-lg font-bold mb-4">Quick Links</h3>
                    <ul class="space-y-2">
                        <li><a href="../#home" class="text-purple-300 hover:text-white text-sm">Home</a></li>
                        <li><a href="../#services" class="text-purple-300 hover:text-white text-sm">Services</a></li>
                        <li><a href="../#resources" class="text-purple-300 hover:text-white text-sm">Resources</a></li>
                        <li><a href="../#events" class="text-purple-300 hover:text-white text-sm">Events</a></li>
                        <li><a href="../#about" class="text-purple-300 hover:text-white text-sm">About Us</a></li>
                    </ul>
                </div>
              
                <div>
                    <h3 class="font-serif text-lg font-bold mb-4">Contact Us</h3>
                    <ul class="space-y-2 text-purple-300 text-sm">
                        <li>Tres Ladson</li>
                        <li><a href="#" onclick="openEmail()">Admin@tlcfamilyservices.com</a></li>
                        <li><a href="#" onclick="openCallPopup()">667-355-2334</a></li>
                        <li>Online-based services</li>
                    </ul>
                </div>
              
                <div>
                    <h3 class="font-serif text-lg font-bold mb-4">Follow Us</h3>
                    <div class="flex space-x-4">
                        <a href="https://www.instagram.com/tlc_familyservices?igsh=MTg5NTNva3lidGMxeg==" class="text-purple-300 hover:text-white">
                            <i class="fab fa-instagram text-xl"></i>
                        </a>
                    </div>
                  
                    <h3 class="font-serif text-lg font-bold mt-6 mb-3">Subscribe to Newsletter</h3>
                    <form class="flex">
                        <input type="email" placeholder="Your email" class="px-4 py-2 rounded-l-lg text-purple-900 w-full">
                        <button type="submit" class="bg-purple-600 hover:bg-purple-700 px-4 py-2 rounded-r-lg transition duration-300"><i class="fas fa-paper-plane text-white"></i></button>
                    </form>
                </div>
            </div>
          
            <div class="border-t border-purple-800 pt-8 flex flex-col md:flex-row justify-between items-center">
                <p class="text-purple-300 text-sm mb-4 md:mb-0">© 2023 TLC Family Services. All rights reserved.</p>
                <div class="flex space-x-6">
                    <a href="#" onclick="openPrivacy()" class="text-purple-300 hover:text-white text-sm">Privacy Policy</a>
                    <a href="#" onclick="openTerms()" class="text-purple-300 hover:text-white text-sm">Terms of Service</a>
                    <a href="#" class="text-purple-300 hover:text-white text-sm">HIPAA Compliance</a>
                </div>
            </div>
          
            <div class="mt-4 text-center md:text-left">
                <p class="text-purple-400 text-xs italic">TLC Family Services does not provide emergency care. If you're in crisis, call 988 or go to your nearest emergency room.</p>
            </div>
        </div>
    </footer>

    <!-- Privacy Policy Modal -->
    <div id="privacy-modal" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <h3 class="font-serif text-2xl font-bold text-purple-800 mb-6">Privacy Policy</h3>
            <p class="text-pink-700">
                At TLC Family Services, your privacy is our priority. In compliance with U.S. health laws like HIPAA, we safeguard your personal health information (PHI) with encrypted storage and secure communications. We only share data with your consent for treatment, payment, or operations. You have rights to access, amend, or restrict your information. We never sell data and use it only for care delivery. For full details, contact us. This policy ensures trust in your healing journey.
            </p>
        </div>
    </div>

    <!-- Terms of Service Modal -->
    <div id="terms-modal" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <h3 class="font-serif text-2xl font-bold text-purple-800 mb-6">Terms of Service</h3>
            <p class="text-pink-700">
                By using TLC Family Services, you agree to our terms. We provide virtual therapy in compliance with U.S. health regulations, including confidentiality under HIPAA. Services are for informational and therapeutic purposes; not for emergencies (call 911 or 988). Payment terms: Sessions are billed per agreement; cancellations require 24-hour notice or fees apply. We reserve the right to terminate services if guidelines aren't followed. Your participation is voluntary, and we're committed to ethical care. Contact us for questions.
            </p>
        </div>
    </div>

    <!-- Call Popup Modal -->
    <div id="call-modal" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <h3 class="font-serif text-2xl font-bold text-purple-800 mb-6">Call Us</h3>
            <p class="text-pink-700 text-center">667-355-2334</p>
        </div>
    </div>

    <script>
        // Mobile menu toggle
        document.getElementById('mobile-menu-button').addEventListener('click', function() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        });

        // Open email client
        function openEmail() {
            window.location.href = "mailto:Admin@tlcfamilyservices.com";
        }

        // Open call popup and dialer
        function openCallPopup() {
            document.getElementById('call-modal').style.display = "block";
            window.location.href = "tel:667-355-2334";
        }

        // Open Privacy modal
        function openPrivacy() {
            document.getElementById('privacy-modal').style.display = "block";
        }

        // Open Terms modal
        function openTerms() {
            document.getElementById('terms-modal').style.display = "block";
        }

        // Close modals
        document.querySelectorAll('.close').forEach(closeBtn => {
            closeBtn.addEventListener('click', function() {
                this.parentElement.parentElement.style.display = "none";
            });
        });
        window.addEventListener('click', function(event) {
            if (event.target.classList.contains('modal')) {
                event.target.style.display = "none";
            }
        });

        // Async submission
        document.getElementById('additional-consent-form').addEventListener('submit', async function(e) {
            e.preventDefault();
            const status = document.getElementById('status_additional');
            const data = new FormData(e.target);
            fetch(e.target.action, {
                method: 'POST',
                body: data,
                headers: {
                    'Accept': 'application/json'
                }
            }).then(response => {
                if (response.ok) {
                    status.innerHTML = "Thanks for your submission!";
                    e.target.reset();
                } else {
                    response.json().then(data => {
                        status.innerHTML = data.errors ? data.errors.map(error => error.message).join(", ") : "Oops! Problem submitting form.";
                    });
                }
            }).catch(error => {
                status.innerHTML = "Oops! Problem submitting form.";
            });
        });

        // Print function
        function printForm(content) {
            content.classList.add('print-area');
            window.print();
            content.classList.remove('print-area');
        }
    </script>
</body>
</html>
