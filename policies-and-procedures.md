<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Policies and Procedures - TLC Family Services</title>
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
        .policy-section {
            scroll-margin-top: 100px;
        }
        .nav-link.active {
            color: #3b82f6;
            font-weight: 600;
        }
        .signature-box {
            border-bottom: 1px solid #000;
            display: inline-block;
            min-width: 300px;
            margin-top: 30px;
        }
        @media print {
            .no-print {
                display: none;
            }
            body {
                font-size: 12pt;
            }
            .policy-section {
                page-break-inside: avoid;
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

    <div class="container mx-auto px-4 py-8">
        <div class="flex flex-col lg:flex-row gap-8">
            <!-- Navigation Sidebar -->
            <nav class="lg:w-1/4 bg-white p-6 rounded-lg shadow-md h-fit sticky top-4 no-print">
                <h2 class="font-serif text-xl font-bold mb-4 text-purple-800 border-b pb-2">Policy Sections</h2>
                <ul class="space-y-2">
                    <li><a href="#introduction1" class="nav-link block hover:text-purple-600 transition">Introduction</a></li>
                    <li><a href="#psychotherapy1" class="nav-link block hover:text-purple-600 transition">Psychotherapy Services</a></li>
                    <li><a href="#confidentiality1" class="nav-link block hover:text-purple-600 transition">Confidentiality</a></li>
                    <li><a href="#sessions1" class="nav-link block hover:text-purple-600 transition">Session Policies</a></li>
                    <li><a href="#telehealth1" class="nav-link block hover:text-purple-600 transition">Telehealth/Video</a></li>
                    <li><a href="#insurance1" class="nav-link block hover:text-purple-600 transition">Insurance Coverage</a></li>
                    <li><a href="#records1" class="nav-link block hover:text-purple-600 transition">Client Records</a></li>
                    <li><a href="#payment1" class="nav-link block hover:text-purple-600 transition">Payment Policies</a></li>
                    <li><a href="#minors1" class="nav-link block hover:text-purple-600 transition">Child/Adolescent Clients</a></li>
                    <li><a href="#contact1" class="nav-link block hover:text-purple-600 transition">Contacting Your Therapist</a></li>
                    <li><a href="#cancellation1" class="nav-link block hover:text-purple-600 transition">Cancellation Policy</a></li>
                    <li><a href="#office1" class="nav-link block hover:text-purple-600 transition">Office Visits</a></li>
                    <li><a href="#communication1" class="nav-link block hover:text-purple-600 transition">Text/Email Policy</a></li>
                    <li><a href="#crisis1" class="nav-link block hover:text-purple-600 transition">Crisis Procedures</a></li>
                    <li><a href="#court1" class="nav-link block hover:text-purple-600 transition">Court Matters</a></li>
                    <li><a href="#signatures1" class="nav-link block hover:text-purple-600 transition">Signatures</a></li>
                </ul>
            </nav>

            <!-- Policy Content -->
            <div class="lg:w-3/4 bg-white p-8 rounded-lg shadow-md">
                <div class="text-center mb-8">
                    <h1 class="font-serif text-3xl font-bold text-purple-800 mb-2">Policy and Procedures</h1>
                    <p class="text-pink-700">Last Updated: <span id="current-date1"></span></p>
                </div>

                <form id="acknowledgment-form1" action="https://formspree.io/f/mzzvjdow" method="POST" class="space-y-6">

                <!-- Introduction Section -->
                <section id="introduction1" class="policy-section mb-12">
                    <h2 class="font-serif text-2xl font-bold text-purple-800 mb-4 border-b pb-2">Introduction</h2>
                    <div class="space-y-4 text-pink-700">
                        <p>TLC Family Services is a group practice of individual clinicians who provide mental health/behavioral health services to clients who are seeking support to address their emotional needs, health, and wellness.</p>
                        <p>Each clinician is an independent practitioner practicing within his/her scope of expertise within the group. Upon meeting with the clinician, the client will provide relevant information about him/herself as well as discuss his/her presenting concern with the clinician. The clinician will ask specific questions regarding the client's background and present concern to as a part of the diagnostic process.</p>
                        <p>Generally, the Intake is completed during the first meeting; however, in some instances, depending on history and presenting concerns, the Intake may extend over the course of 2 or more sessions to eminently form an appropriate mental health diagnosis and make a recommendation for treatment. The clinician will explain to you the mental health diagnosis as well as work with you to create an appropriate treatment to address your needs and concerns.</p>
                    </div>
                </section>

                <!-- Psychotherapy Services Section -->
                <section id="psychotherapy1" class="policy-section mb-12">
                    <h2 class="font-serif text-2xl font-bold text-purple-800 mb-4 border-b pb-2">Psychotherapy and Counseling Services</h2>
                    <div class="space-y-4 text-pink-700">
                        <p>Psychotherapy is a broad term that is difficult to fully define. The process of psychotherapy and interventions used by the clinician will vary based on the training and expertise of the clinician and the issues/concerns presented by the client.</p>
                        <p>For psychotherapy to reach its full potential benefits it is necessarily for the client to actively participate in his/her treatment. The clinician will encourage active participation but will not attempt to force or manage a client's participation or active engagement. The expectation is the client will work on things discussed in sessions during session time as well as outside of session (this may include completing therapeutic homework assignments).</p>
                        <p>It is important to understand that the potential benefits and risks of engaging in psychotherapy are specific to everyone. Therapy often involves discussing unpleasant experiences, struggles, concerns, etc and as such may, at times, elicit negative feelings for the individual. However, effective psychotherapy offers many potential benefits that may guide the individual toward electively managing/regulating his/her emotional experience, solving specific problems, improving functioning and behavior reducing conflict and stress, and establishing healthier relationships.</p>
                        <p class="font-semibold bg-purple-50 p-3 rounded border-l-4 border-purple-400">There are no guarantees of what each individual will experience.</p>
                    </div>
                </section>

                <!-- Confidentiality Section -->
                <section id="confidentiality1" class="policy-section mb-12">
                    <h2 class="font-serif text-2xl font-bold text-purple-800 mb-4 border-b pb-2">Office Policies: Confidentiality</h2>
                    <div class="space-y-4 text-pink-700">
                        <p>The issues you discuss in psychotherapy with your therapist are confidential and cannot be disclosed without your knowledge or written consent. However, there are some exceptions to confidentiality as mandated by State and Federal laws and are stated in our Confidentiality and Limits of Confidentiality Policy that you will review and sign prior to commencing treatment.</p>
                        <p>All therapists endeavor to maintain the confidentiality of their clients and adhere to state and federal laws, and professional ethical guidelines in maintaining the standards of confidentiality. Your records will not be sent or shown to others (except for your insurance company) without a signed release from you. In such cases, your therapist will release the minimum amount of information to satisfy the insurance company under the terms of the Health Insurance Portability and Accountability Act (HIPAA) of 1996. Please refer to our Notice of Privacy Standards for details.</p>
                        <p>All client records are maintained and securely stored in the offices of TLC Family Services. Client records are only accessible to your therapist and TLC Family Services and administrators.</p>
                    </div>
                </section>

                <!-- Session Policies Section -->
                <section id="sessions1" class="policy-section mb-12">
                    <h2 class="font-serif text-2xl font-bold text-purple-800 mb-4 border-b pb-2">Office Policies: Sessions</h2>
                    <div class="space-y-4 text-pink-700">
                        <p>Therapy sessions are conducted in the office, telehealth, video, and in home at an agreed upon session time. Sessions are generally 30-60 minutes for psychotherapy and 15 min for medication management in duration unless otherwise specified. In home sessions are based on the individual need of the client and are subject to change at any time.</p>
                    </div>
                </section>

                <!-- Telehealth Section -->
                <section id="telehealth1" class="policy-section mb-12">
                    <h2 class="font-serif text-2xl font-bold text-purple-800 mb-4 border-b pb-2">Office Policies: Telehealth/Video</h2>
                    <div class="space-y-4 text-pink-700">
                        <p>Telehealth/Video is a specific type of service delivery of counseling services that is offered at TLC currently. As we guarantee the confidentiality or privacy of each session, we offer telephone or other electronic forms of sessions via platform.</p>
                        <p>To provide such services, the practice is required to have special software, policies and procedures, and operational equipment to meet the appropriate standards of practice and regulations under State and Federal Laws and guidelines established by State Managed Care Organizations and Insurance.</p>
                    </div>
                </section>

                <!-- Insurance Coverage Section -->
                <section id="insurance1" class="policy-section mb-12">
                    <h2 class="font-serif text-2xl font-bold text-purple-800 mb-4 border-b pb-2">Office Policies: Insurance Coverage</h2>
                    <div class="space-y-4 text-pink-700">
                        <p>Client agrees to notify the therapist of any changes in insurance coverage. If your insurance changes for any reason the therapist must know prior to the next scheduled session. The practice is required to verify insurance benefits and coverage before providing services. In the event your insurance coverage changes or is cancelled and/or you do not provide notice you are financially responsible for all services rendered not covered because of changes to your coverage or benefit eligibility.</p>
                        <p>Failure to pay for services rendered will result in a suspension or termination of therapeutic services. Services may resume when the client's account is paid in full to date.</p>
                        <p>Prior to the commencement of services, we will contact you (via email with your permission) and inform you of confirmation of your insurance benefits and eligibility for outpatient mental health service. You will be notified of your co-pay, deductible, and/or co-insurance obligation prior to the Intake session. Payment is required at the time services are rendered.</p>
                        <p>Additionally, our office staff conducts insurance eligibility checks for all active clients on a regular basis. In the event we discover a change in your coverage we will notice you immediately. Our goal is to prevent any disruption in your counseling services if possible. If your insurance benefits term or your coverage changes to an out of network plan, we will work you to provide options to continue services or offer referral information to an in-network provider.</p>
                        <p>To utilize insurance benefits for mental health/behavioral health services, the therapist must indicate that it is medically necessary to do so. In order to meet this standard, the therapist will evaluate the client and offer a mental health diagnosis congruent with presented issues/concerns, functioning, etc. This information, along with the date, duration and type of session will be disclosed to the insurance company for reimbursement purposes.</p>
                        <p>In some cases, the insurance company may request a copy of the client's medical records to review the necessity of services, audit service delivery, etc. as they are the payer of services, we are contractually obligated to fulfill such a request. If this was to occur, the therapist will notify the client of the request.</p>
                    </div>
                </section>

                <!-- Client Records Section -->
                <section id="records1" class="policy-section mb-12">
                    <h2 class="font-serif text-2xl font-bold text-purple-800 mb-4 border-b pb-2">Office Policies: Client Records</h2>
                    <div class="space-y-4 text-pink-700">
                        <p>All client records are secured and maintained by TLC. Client records are not released to third parties without the written consent of the client (and/or parent/guardian of the client). The only exception to this is if your insurance company requests to inspect your record or we receive a court order to do so.</p>
                        <p>If you consent for your records to be released to a third party we will only release your Intake Summary, Treatment Plans, and Discharge Summary to the third party. Session notes, psychotherapy notes, and other documentation will not be released.</p>
                        <p>You have the right to inspect your client records at any time; such requests should be made in writing and submitted to the administrator. Inspection of the file may occur at our office. If you request a paper copy of your client record a charge of $0.25/page will be applied and payment is required when you pick up your records.</p>
                        <p>We will only release a copy of the record to the actual client (parent/guardian) in person upon receipt of payment and proof of identity. Client records will not be mailed. If a medical hardship exists that prevents you from picking up your record, we will make arrangements to have it sent certified mail; client is responsible for the cost of postage and agrees to indemnify TLC Family Services of liability for lost or stolen records that are mail upon the client's request.</p>
                    </div>
                </section>

                <!-- Payment Policies Section -->
                <section id="payment1" class="policy-section mb-12">
                    <h2 class="font-serif text-2xl font-bold text-purple-800 mb-4 border-b pb-2">Office Policies: Payment for Services</h2>
                    <div class="space-y-4 text-pink-700">
                        <p>Client understands that payment and/or applicable service fees are expected at the time of service. Upon agreement between the client and therapist, a service fee may be paid at the client's next scheduled session; however, further delay of payment may result in the termination or suspension of services.</p>
                        <p>Payment may be made in the form of Cash, Check (rendered payable to TLC Family Services), or Money Order (rendered payable to TLC Family Services), a service fee of $35.00 will be processed for any returned checks. After a second returned check the client will be required to pay for services with Cash or Money Order only.</p>

                        <h3 class="text-xl font-semibold mt-6 mb-2 text-purple-600">Failure to Pay</h3>
                        <p>Client agrees to keep his/her account in good standing and pay all applicable fees in a timely manner. Client understands that failure to pay for services rendered will result in a suspension or termination of therapeutic services. Services may resume when the client's account is paid in full to date.</p>
                    </div>
                </section>

                <!-- Child/Adolescent Clients Section -->
                <section id="minors1" class="policy-section mb-12">
                    <h2 class="font-serif text-2xl font-bold text-purple-800 mb-4 border-b pb-2">Office Policies: Child and Adolescent Clients</h2>
                    <div class="space-y-4 text-pink-700">
                        <p>Any child/adolescent under the age of 14 must have the permission of both parents/guardians to participate in treatment unless there is a legal custody agreement stating otherwise. In addition, adolescents age 14 and older control their own records and confidentiality is enforced even with parents/guardians; specific release forms must be signed by the adolescent client in order to discuss treatment issues.</p>
                        <p>Parents/Guardians are encouraged to support the confidentiality between the therapist and their child. As well, it is important to understand that any communication between the therapist and parent/guardian will be shared with the child to maintain trust and emotional safety within the therapeutic alliance.</p>
                        <p>No child under the age of 15 may be left unattended by a parent/guardian in the waiting room. In addition, a parent/guardian must remain in the building or on premises during the child's session (child under the age of 15). Please be advised that TLC Family Services and individual therapists are not responsible for supervising or monitoring children who are left unattended or dropped off to session.</p>
                    </div>
                </section>

                <!-- Contacting Your Therapist Section -->
                <section id="contact1" class="policy-section mb-12">
                    <h2 class="font-serif text-2xl font-bold text-purple-800 mb-4 border-b pb-2">Office Policies: Contacting Your Therapist</h2>
                    <div class="space-y-4 text-pink-700">
                        <p>Due to the nature of the services provided it is often difficult for therapists to be immediately available by telephone. Most often, it is likely you will get voicemail when calling your therapist or the office. Therapists do not answer calls when they are with other clients.</p>
                        <p>If your call is answered by voicemail, please leave a message; if calling the office please leave your name and the name of the therapist you are calling for. Your therapist will make every effort to return your call the same day or within 24-48 business hours (except for weekends and holidays).</p>
                        <p>If your therapist is unavailable for an extended period (more than one week) you will be provided the name and contact information of a professional colleague who will address your concerns in your therapist's absence, if needed.</p>
                    </div>
                </section>

                <!-- Cancellation Policy Section -->
                <section id="cancellation1" class="policy-section mb-12">
                    <h2 class="font-serif text-2xl font-bold text-purple-800 mb-4 border-b pb-2">Office Policies: Cancellation/No Show</h2>
                    <div class="space-y-4 text-pink-700">
                        <p>Client agrees to provide 24-hour notice of any need to cancel a scheduled session. It is understood that this is not always possible as illness can occur at any time; however, if multiple sessions are missed (no show/no call) or cancelled at the last minute it is difficult to reschedule and will interfere with continuity of care.</p>
                        <p>After the first no show/no call the client will be charged for the missed session. The cost assessed is $65.00. This is not covered by insurance. Under State regulation and agreement with MCO this fee cannot be assessed to clients who have Medical Assistance.</p>
                        <p>Consistent no show/no call or last-minute cancellations (more than 2 in a 4-week period) may result in termination of services – this is applicable to all clients regardless of payment and insurance coverage type.</p>
                    </div>
                </section>

                <!-- Office Visits Section -->
                <section id="office1" class="policy-section mb-12">
                    <h2 class="font-serif text-2xl font-bold text-purple-800 mb-4 border-b pb-2">Office Policies: In Office Visits/Waiting Room</h2>
                    <div class="space-y-4 text-pink-700">
                        <p>Upon arrival, clients are asked to wait in the waiting room until their therapist greets them. Clients may use the restroom if needed but otherwise should not leave the waiting room unless accompanied by a therapist. Please do not knock on doors while the therapist is in session as this will disrupt services to another client. If he/she is running late, please be patient (allow 5-10 minutes); if he/she does not greet you within a reasonable amount of time please call your therapist or the office for assistance.</p>
                        <p>No child under the age of 15 may be left unattended by a parent/guardian in the waiting room in addition, a parent/guardian must remain in the office waiting room or on premise during the child's session (child under the age of 15). TLC and individual therapists are not responsible for supervising or monitoring children who are left unattended or dropped off to session. Failure of the parent/guardian to adhere to this policy may result in the termination of services to the client.</p>
                        <p>If a parent/guardian would like to discuss something with the therapist and prefer the child not be present, the therapist will make an effort to find an available office to have the discussion while allowing the child to remain in his/her office. If this is not possible, arrangements may be made to speak with the therapist at another time.</p>
                        <p>Clients and visitors are prohibited to bringing drugs, alcohol, and/or weapons into the office. If a client or visitor is discovered to have any of these prohibited items in his/her possession he/she will be asked to leave the premise immediately. Any client who violates this policy will be immediately terminated for services and notified by an administrator of TLC Family Services of such within 24 business hours of the incident. Any client or visitor that appears to be impaired and under the influence of a substance will be assisted as appropriate; if necessary, law enforcement may be contacted to assist with such a situation.</p>
                        <p>Clients and visitors are asked to refrain from making excessive noise or causing a disruption to others while in the waiting room. In addition, it is requested that individuals not discuss topics of a personal nature as this may create discomfort and/or concern for others in the waiting room. To provide a comforting, safe, and pleasant atmosphere we ask that all clients be respectful of this policy.</p>
                    </div>
                </section>

                <!-- Text/Email Policy Section -->
                <section id="communication1" class="policy-section mb-12">
                    <h2 class="font-serif text-2xl font-bold text-purple-800 mb-4 border-b pb-2">Office Policies: Text Messaging and Email</h2>
                    <div class="space-y-4 text-pink-700">
                        <p>If agreed upon at the commencement of services, text messaging and email may be used as a means of communication between the client and the therapist. This can be done using the patient portal or text messages.</p>
                        <p>The therapist will accept and respond to text messages and emails re: scheduling sessions, confirming sessions, rescheduling sessions, or canceling sessions. Please do not text or email confidential treatment information to your therapist, confidentiality cannot be guaranteed, as these platforms are not encrypted. Text messages or emails received that include treatment concerns or other confidential information will be deleted; this policy is to protect your confidentiality.</p>
                    </div>
                </section>

                <!-- Crisis Procedures Section -->
                <section id="crisis1" class="policy-section mb-12">
                    <h2 class="font-serif text-2xl font-bold text-purple-800 mb-4 border-b pb-2">Office Policies: Crisis</h2>
                    <div class="space-y-4 text-pink-700">
                        <p>In the event of an emergency, you should text 988 Suicide and Crisis Lifeline or the National Hotline for Mental Health Crises And Suicide Prevention at 800-273-TALK (8255). In the event of a life-threatening emergency please call 911 immediately or go to your nearest emergency room.</p>
                        <p>If you are admitted for crisis intervention your therapist will communicate with the crisis center or hospital with the client's written consent.</p>
                    </div>
                </section>

                <!-- Court Matters Section -->
                <section id="court1" class="policy-section mb-12">
                    <h2 class="font-serif text-2xl font-bold text-purple-800 mb-4 border-b pb-2">Office Policies: Court Related Matters</h2>
                    <div class="space-y-4 text-pink-700">
                        <p>The independent practitioners at TLC do not offer legal advice, complete or submit third party form/correspondence, nor do they participate in Court-related matters, such as, but not limited to: divorce, custody matters, worker compensation/disability, and/or criminal matters, unless otherwise arranged PRIOR TO the commencement of services.</p>
                    </div>
                </section>

                <!-- Signature Section -->
                <section id="signatures1" class="policy-section">
                    <div class="space-y-4 text-pink-700">
                        <p>The client should retain a copy of this document for his/her records and reference.</p>

                        <div class="mt-8">
                            <div class="flex justify-between">
                                <div>
                                    <p>Independent Practitioner Signature and Credentials:</p>
                                    <div class="signature-box font-bold">Pre-signed by Practitioner</div>
                                </div>
                                <div class="text-right">
                                    <p>Client/Parent/Guardian Signature:</p>
                                    <input type="text" name="client_signature" class="border-b border-purple-300 w-full py-2 focus:outline-none focus:border-purple-500" placeholder="Type your full name as signature">
                                    <p class="mt-2">Date: <input type="date" name="date" class="border-b border-purple-300 py-2 focus:outline-none focus:border-purple-500"></p>
                                </div>
                            </div>

                            <div class="mt-8">
                                <div class="flex items-center">
                                    <input type="checkbox" name="received_copy" id="received_copy1" class="mr-2">
                                    <label for="received_copy1">Client (or Parent/Guardian) was provided a signed copy of this document.</label>
                                </div>
                                <div class="flex items-center mt-2">
                                    <input type="checkbox" name="declined_copy" id="declined_copy1" class="mr-2">
                                    <label for="declined_copy1">Client (or Parent/Guardian) declined a signed copy of this document.</label>
                                </div>
                            </div>
                        </div>
                    </div>
                </section>

                <div class="flex space-x-4">
                    <button type="submit" class="flex-1 bg-purple-600 hover:bg-purple-700 text-white font-medium py-3 px-4 rounded-lg transition duration-300">Submit Acknowledgment</button>
                    <button type="button" onclick="printForm(document.body)" class="flex-1 bg-pink-500 hover:bg-pink-600 text-white font-medium py-3 px-4 rounded-lg transition duration-300">Print Copy</button>
                </div>
                <p id="status1" class="mt-4 text-sm text-pink-600 text-center"></p>
            </form>
            </div>
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

        // Set current date
        document.getElementById('current-date1').textContent = new Date().toLocaleDateString('en-US', {
            year: 'numeric',
            month: 'long',
            day: 'numeric'
        });

        // Highlight active nav link
        const sections = document.querySelectorAll('.policy-section');
        const navLinks = document.querySelectorAll('.nav-link');

        window.addEventListener('scroll', () => {
            let current = '';

            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                const sectionHeight = section.clientHeight;

                if (pageYOffset >= (sectionTop - 150)) {
                    current = section.getAttribute('id');
                }
            });

            navLinks.forEach(link => {
                link.classList.remove('active');
                if (link.getAttribute('href') === `#${current}`) {
                    link.classList.add('active');
                }
            });
        });

        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();

                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);

                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 100,
                        behavior: 'smooth'
                    });
                }
            });
        });

        // Async submission
        document.getElementById('acknowledgment-form1').addEventListener('submit', async function(e) {
            e.preventDefault();
            const status = document.getElementById('status1');
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
