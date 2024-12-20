<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Main Page</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.1.3/css/bootstrap.min.css" rel="stylesheet">
    <style>
        /* Custom Style for Navbar */
        .navbar {
            background-color: rgb(214, 231, 253) !important;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        body {
            background-color: rgba(248, 248, 248, 0.99);
        }

        /* Profile Container Styling */
        .profile-container {
            width: 300px;
            margin: 20px;
            padding: 0;
            /* No padding here, the internal sections will handle padding */
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            text-align: center;
            float: left;
            overflow: hidden;
        }

        /* Top Section of Profile Container (Blue) */
        .profile-container .top-section {
            background-color: rgb(214, 231, 253);
            /* Blue Color */
            padding: 20px;
        }

        /* Bottom Section of Profile Container (White) */
        .profile-container .bottom-section {
            background-color: white;
            /* White Color */
            padding: 20px;
        }

        .profile-container img {
            border-radius: 50%;
            margin-bottom: 15px;
        }

        .profile-container a {
            display: block;
            font-size: 1.00rem;
            font-weight: bold;
            color: rgb(0, 0, 0);
            text-decoration: none;
        }
    </style>
</head>

<body>

    <div class="container-fluid">
        <div class="row">
            <!-- Main Content Area -->
            <div class="col-md-12">
                <!-- Navigation Bar -->
                <nav class="navbar navbar-expand-lg navbar-light">
                    <div class="container-fluid d-flex justify-content-between align-items-center">
                        <!-- Dropdown Menu on the Left -->
                        <div class="dropdown">
                            <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenuButton" data-bs-toggle="dropdown" aria-expanded="false">
                                =
                            </button>
                            <ul class="dropdown-menu" aria-labelledby="dropdownMenuButton">
                                <li><a class="dropdown-item" href="#">Dashboard</a></li>
                                <li><a class="dropdown-item" href="<?= site_url('studentprofile') ?>">Student Profile</a></li>
                                <li><a class="dropdown-item" href="<?= site_url('academic') ?>">Academic</a></li>
                                <li><a class="dropdown-item" href="<?= site_url('finance') ?>">Finance</a></li>
                            </ul>
                        </div>

                        <!-- Logo and UPSI EduAnalytic Dashboard -->
                        <div class="d-flex align-items-center">
                            <img src="<?= base_url('assets/images/5.png') ?>" style="width:15%; height:auto; margin-right: 10px;">
                            <a class="navbar-brand fw-bold" href="#">UPSI EduAnalytic Dashboard</a>
                        </div>

                        <!-- Right-aligned Home and Logout -->
                        <div class="navbar-nav">
                            <!-- Navigation Bar Home Link (Bold) -->
                            <a class="nav-link fw-bold" href="<?= site_url('home_controller') ?>">Home</a>
                            <a class="nav-link fw-bold" href="#">Logout</a>
                        </div>
                    </div>
                </nav>

                <!-- Profile Container with Two Color Division -->
                <div class="profile-container">
                    <!-- Top Section (Blue) -->
                    <div class="top-section">
                        <img src="<?= base_url('assets/images/6.png') ?>" style="width:100px; height:150px; border-radius: 100%; border: 5px rgb(214, 231, 253);" alt="Profile Picture">
                        <a href="#">Nama Advisor</a>
                    </div>

                    <!-- Bottom Section (White) -->
                    <div class="bottom-section">
                        <a href="#">Fakulti</a>
                        <a href="#">Email</a>
                        <a href="#">Num.telefon</a>
                    </div>
                </div>

                <!-- Main Content Section -->
                <div class="content" style="margin-left: 320px;">
                    <h1>Welcome to the Main Page!</h1>
                    <p>Additional content can go here, aligned to the right of the profile container.</p>
                </div>
            </div>
        </div>

        <!-- Footer (optional) -->
        <footer class="bg-light text-center mt-5 p-3">
            <p>&copy; 2024 UPSI EduAnalytic Dashboard</p>
        </footer>
    </div>

    <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.1.3/js/bootstrap.bundle.min.js"></script>
</body>

</html>
