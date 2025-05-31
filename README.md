<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Smart Strom - Professionelle Elektroinstallationen</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700&family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
    <style>
        /* Stylowanie jak w poprzednim przykładzie, ale zoptymalizowane pod język niemiecki */
        :root {
            --primary: #0d6efd;
            --primary-dark: #0b5ed7;
            --energy-green: #28a745;
            --tech-blue: #007bff;
            --light: #f8f9fa;
            --dark: #212529;
            --gray: #6c757d;
            --success: #198754;
            --danger: #dc3545;
            --shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            --transition: all 0.3s ease;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Open Sans', sans-serif;
            color: var(--dark);
            line-height: 1.6;
            background-color: #f0f4f8;
        }

        h1, h2, h3, h4, h5, h6 {
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            margin-bottom: 1rem;
            color: var(--dark);
        }

        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }

        .btn {
            display: inline-block;
            padding: 12px 24px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            transition: var(--transition);
            cursor: pointer;
            border: none;
            font-family: 'Montserrat', sans-serif;
        }

        .btn-primary {
            background-color: var(--primary);
            color: white;
        }

        .btn-primary:hover {
            background-color: var(--primary-dark);
            transform: translateY(-3px);
            box-shadow: var(--shadow);
        }

        .btn-secondary {
            background-color: var(--energy-green);
            color: white;
        }

        .btn-secondary:hover {
            background-color: #218838;
            transform: translateY(-3px);
            box-shadow: var(--shadow);
        }

        /* Language Switcher */
        .language-switcher {
            position: absolute;
            top: 20px;
            right: 20px;
            display: flex;
            gap: 10px;
            z-index: 1001;
        }

        .lang-btn {
            width: 40px;
            height: 30px;
            background-color: rgba(255, 255, 255, 0.8);
            border: 1px solid #ddd;
            border-radius: 4px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition);
        }

        .lang-btn:hover, .lang-btn.active {
            background-color: var(--primary);
            color: white;
            border-color: var(--primary);
        }

        /* Header Styles */
        header {
            background-color: white;
            box-shadow: var(--shadow);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
            position: relative;
        }

        .logo {
            display: flex;
            align-items: center;
        }

        .logo-icon {
            font-size: 2.5rem;
            color: var(--primary);
            margin-right: 10px;
        }

        .logo-text {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--dark);
            display: flex;
            flex-direction: column;
        }

        .logo-text span {
            color: var(--primary);
        }

        .logo-subtitle {
            font-size: 0.8rem;
            font-weight: 500;
            color: var(--gray);
        }

        .nav-menu {
            display: flex;
            list-style: none;
        }

        .nav-menu li {
            margin-left: 25px;
        }

        .nav-menu a {
            text-decoration: none;
            color: var(--dark);
            font-weight: 600;
            transition: var(--transition);
            position: relative;
        }

        .nav-menu a:hover {
            color: var(--primary);
        }

        .nav-menu a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background-color: var(--primary);
            transition: var(--transition);
        }

        .nav-menu a:hover::after {
            width: 100%;
        }

        .mobile-toggle {
            display: none;
            font-size: 1.5rem;
            cursor: pointer;
        }

        /*
