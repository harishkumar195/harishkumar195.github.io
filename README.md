# harishkumar195.github.io
Veterinary Research Portfolio Website
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vet World - Plant-Based Nanoemulsions for Male Antifertility Research</title>
    
    <!-- External Libraries -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Crimson+Text:wght@400;600&display=swap" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    
    <style>
        :root {
            --primary-color: #2c5530;
            --secondary-color: #4a7c59;
            --accent-color: #7cb342;
            --light-green: #e8f5e8;
            --text-dark: #2c3e50;
            --text-light: #7f8c8d;
            --border-light: #e1e8ed;
            --shadow-color: rgba(44, 85, 48, 0.1);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            line-height: 1.6;
            color: var(--text-dark);
            background: linear-gradient(135deg, #f8fffe 0%, #e8f5e8 100%);
        }

        .navbar {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            box-shadow: 0 2px 20px var(--shadow-color);
            transition: all 0.3s ease;
            position: fixed;
            top: 0;
            width: 100%;
            z-index: 1000;
        }

        .navbar-brand {
            font-weight: 700;
            font-size: 1.5rem;
            color: var(--primary-color) !important;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .nav-link {
            color: var(--text-dark) !important;
            font-weight: 500;
            transition: all 0.3s ease;
            padding: 0.5rem 1rem !important;
            border-radius: 8px;
        }

        .nav-link:hover, .nav-link.active {
            background: var(--light-green);
            color: var(--primary-color) !important;
            transform: translateY(-2px);
        }

        .hero-section {
            background: linear-gradient(135deg, var(--primary-color) 0%, var(--secondary-color) 100%);
            color: white;
            padding: 120px 0 80px;
            margin-top: 76px;
            position: relative;
            overflow: hidden;
        }

        .hero-section::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><defs><pattern id="grain" width="100" height="100" patternUnits="userSpaceOnUse"><circle cx="25" cy="25" r="1" fill="white" opacity="0.1"/><circle cx="75" cy="75" r="1" fill="white" opacity="0.1"/><circle cx="50" cy="10" r="0.5" fill="white" opacity="0.05"/><circle cx="10" cy="60" r="0.5" fill="white" opacity="0.05"/></pattern></defs><rect width="100" height="100" fill="url(%23grain)"/></svg>');
            opacity: 0.3;
        }

        .hero-content {
            position: relative;
            z-index: 2;
        }

        .hero-title {
            font-family: 'Crimson Text', serif;
            font-size: 3rem;
            font-weight: 600;
            margin-bottom: 1.5rem;
            line-height: 1.2;
        }

        .hero-subtitle {
            font-size: 1.2rem;
            opacity: 0.9;
            margin-bottom: 2rem;
        }

        .section-padding {
            padding: 80px 0;
        }

        .section-title {
            font-family: 'Crimson Text', serif;
            font-size: 2.5rem;
            font-weight: 600;
            color: var(--primary-color);
            margin-bottom: 3rem;
            text-align: center;
            position: relative;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: linear-gradient(90deg, var(--primary-color) 0%, var(--accent-color) 100%);
            border-radius: 2px;
        }

        .card-modern {
            background: rgba(255, 255, 255, 0.9);
            border: none;
            border-radius: 20px;
            box-shadow: 0 10px 40px var(--shadow-color);
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
            margin-bottom: 30px;
        }

        .card-modern:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 60px rgba(44, 85, 48, 0.15);
        }

        .card-header-modern {
            background: linear-gradient(135deg, var(--primary-color) 0%, var(--secondary-color) 100%);
            color: white;
            border: none;
            border-radius: 20px 20px 0 0;
            padding: 1.5rem 2rem;
            font-weight: 600;
            font-size: 1.1rem;
        }

        .info-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-bottom: 50px;
        }

        .info-card {
            background: rgba(255, 255, 255, 0.9);
            padding: 2rem;
            border-radius: 15px;
            box-shadow: 0 5px 25px var(--shadow-color);
            transition: all 0.3s ease;
            border-left: 5px solid var(--accent-color);
        }

        .info-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 40px rgba(44, 85, 48, 0.15);
        }

        .info-label {
            font-weight: 600;
            color: var(--primary-color);
            margin-bottom: 0.5rem;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .info-value {
            color: var(--text-dark);
            font-size: 1.1rem;
        }

        .abstract-section {
            background: rgba(255, 255, 255, 0.9);
            padding: 3rem;
            border-radius: 20px;
            box-shadow: 0 10px 40px var(--shadow-color);
            margin: 50px 0;
            text-align: justify;
            line-height: 1.8;
        }

        .keywords-container {
            margin-top: 2rem;
        }

        .keyword-tag {
            display: inline-block;
            background: var(--light-green);
            color: var(--primary-color);
            padding: 8px 16px;
            border-radius: 25px;
            margin: 5px 8px 5px 0;
            font-weight: 500;
            font-size: 0.9rem;
            border: 2px solid transparent;
            transition: all 0.3s ease;
        }

        .keyword-tag:hover {
            border-color: var(--accent-color);
            transform: scale(1.05);
        }

        .author-card {
            background: linear-gradient(135deg, var(--primary-color) 0%, var(--secondary-color) 100%);
            color: white;
            padding: 2rem;
            border-radius: 20px;
            text-align: center;
            margin: 40px 0;
        }

        .orcid-link {
            color: #a6ce39;
            text-decoration: none;
            font-weight: 600;
            display: inline-flex;
            align-items: center;
            gap: 8px;
            transition: all 0.3s ease;
        }

        .orcid-link:hover {
            color: #fff;
            transform: scale(1.05);
        }

        .chart-container {
            position: relative;
            background: rgba(255, 255, 255, 0.9);
            padding: 2rem;
            border-radius: 15px;
            box-shadow: 0 10px 40px var(--shadow-color);
            margin: 30px 0;
            min-height: 400px;
        }

        .chart-title {
            font-family: 'Crimson Text', serif;
            font-size: 1.5rem;
            font-weight: 600;
            color: var(--primary-color);
            text-align: center;
            margin-bottom: 1.5rem;
        }

        .meta-results {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin: 50px 0;
        }

        .result-card {
            background: rgba(255, 255, 255, 0.9);
            padding: 2rem;
            border-radius: 15px;
            box-shadow: 0 10px 40px var(--shadow-color);
            text-align: center;
            transition: all 0.3s ease;
        }

        .result-card:hover {
            transform: translateY(-5px);
        }

        .result-value {
            font-size: 2rem;
            font-weight: 700;
            color: var(--primary-color);
            margin: 1rem 0;
        }

        .result-label {
            font-weight: 600;
            color: var(--text-dark);
            margin-bottom: 0.5rem;
        }

        .result-ci {
            color: var(--text-light);
            font-size: 0.9rem;
        }

        .contact-section {
            background: linear-gradient(135deg, var(--primary-color) 0%, var(--secondary-color) 100%);
            color: white;
            padding: 60px 0;
            text-align: center;
        }

        .contact-link {
            color: #a6ce39;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.2rem;
            transition: all 0.3s ease;
        }

        .contact-link:hover {
            color: white;
            transform: scale(1.1);
        }

        .btn-scroll-top {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background: var(--primary-color);
            color: white;
            border: none;
            border-radius: 50%;
            width: 60px;
            height: 60px;
            font-size: 1.2rem;
            cursor: pointer;
            transition: all 0.3s ease;
            opacity: 0;
            visibility: hidden;
            z-index: 1000;
        }

        .btn-scroll-top.show {
            opacity: 1;
            visibility: visible;
        }

        .btn-scroll-top:hover {
            background: var(--secondary-color);
            transform: scale(1.1);
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .hero-title {
                font-size: 2rem;
            }
            
            .section-title {
                font-size: 2rem;
            }
            
            .info-grid {
                grid-template-columns: 1fr;
            }
            
            .abstract-section {
                padding: 2rem 1.5rem;
            }
        }

        @media (max-width: 576px) {
            .hero-section {
                padding: 100px 0 60px;
            }
            
            .section-padding {
                padding: 60px 0;
            }
        }

        /* Smooth scrolling */
        html {
            scroll-behavior: smooth;
        }

        /* Animation classes */
        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.6s ease;
        }

        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar navbar-expand-lg navbar-light">
        <div class="container">
            <a class="navbar-brand" href="#home">
                <i class="fas fa-microscope"></i>
                Vet World Research
            </a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link" href="#home">Home</a></li>
                    <li class="nav-item"><a class="nav-link" href="#details">Article Details</a></li>
                    <li class="nav-item"><a class="nav-link" href="#abstract">Abstract</a></li>
                    <li class="nav-item"><a class="nav-link" href="#methods">Methods</a></li>
                    <li class="nav-item"><a class="nav-link" href="#results">Results</a></li>
                    <li class="nav-item"><a class="nav-link" href="#meta-analysis">Meta-Analysis</a></li>
                    <li class="nav-item"><a class="nav-link" href="#discussion">Discussion</a></li>
                    <li class="nav-item"><a class="nav-link" href="#contact">Contact</a></li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero-section">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-lg-10 text-center hero-content">
                    <h1 class="hero-title">Plant-Based Nanoemulsions for Male Antifertility</h1>
                    <p class="hero-subtitle">A Systematic Review and Meta-analysis of Phytochemical Mechanisms and Reproductive Outcomes in Animal Models</p>
                    <div class="d-flex justify-content-center flex-wrap gap-3 mt-4">
                        <span class="badge bg-light text-dark fs-6 px-3 py-2">
                            <i class="fas fa-journal-whills me-2"></i>Veterinary World
                        </span>
                        <span class="badge bg-light text-dark fs-6 px-3 py-2">
                            <i class="fas fa-calendar-alt me-2"></i>November 2025
                        </span>
                        <span class="badge bg-light text-dark fs-6 px-3 py-2">
                            <i class="fas fa-file-alt me-2"></i>Review Article
                        </span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Article Details Section -->
    <section id="details" class="section-padding">
        <div class="container">
            <h2 class="section-title fade-in">Article Details</h2>
            <div class="info-grid">
                <div class="info-card fade-in">
                    <div class="info-label">
                        <i class="fas fa-heading"></i>
                        Article Title
                    </div>
                    <div class="info-value">Plant-Based Nanoemulsions for Male Antifertility: A Systematic Review and Meta-analysis of Phytochemical Mechanisms and Reproductive Outcomes in Animal Models</div>
                </div>
                
                <div class="info-card fade-in">
                    <div class="info-label">
                        <i class="fas fa-journal-whills"></i>
                        Journal Name
                    </div>
                    <div class="info-value">Veterinary World</div>
                </div>

                <div class="info-card fade-in">
                    <div class="info-label">
                        <i class="fas fa-hashtag"></i>
                        Manuscript ID
                    </div>
                    <div class="info-value">2-1764476318</div>
                </div>

                <div class="info-card fade-in">
                    <div class="info-label">
                        <i class="fas fa-file-alt"></i>
                        Manuscript Type
                    </div>
                    <div class="info-value">Review Article</div>
                </div>

                <div class="info-card fade-in">
                    <div class="info-label">
                        <i class="fas fa-calendar-alt"></i>
                        Submission Date
                    </div>
                    <div class="info-value">30-Nov-2025</div>
                </div>

                <div class="info-card fade-in">
                    <div class="info-label">
                        <i class="fas fa-user-md"></i>
                        Author Information
                    </div>
                    <div class="info-value">
                        Harishkumar J. N.<br>
                        <a href="https://orcid.org/0009-0001-0254-2773" target="_blank" class="orcid-link mt-2">
                            <i class="fab fa-orcid"></i>
                            ORCID: 0009-0001-0254-2773
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Abstract Section -->
    <section id="abstract" class="section-padding bg-light">
        <div class="container">
            <h2 class="section-title fade-in">Abstract</h2>
            <div class="abstract-section fade-in">
                <p><strong>Background:</strong> Plant-derived antifertility agents offer promising alternatives to surgical castration and chemical sterilants for controlling male fertility in veterinary species. However, most phytochemicals exhibit limited bioavailability and poor aqueous solubility, reducing their reproductive efficacy. Nanoemulsion technology enhances the delivery, absorption, and testicular penetration of lipophilic herbal compounds, potentially improving antifertility outcomes.</p>

                <p><strong>Aim:</strong> This systematic review and meta-analysis aimed to evaluate the efficacy, mechanisms, and safety of plant-based nanoemulsion formulations used as antifertility agents in male animal models.</p>

                <p><strong>Materials and Methods:</strong> A PRISMA-guided systematic search was conducted across PubMed, Scopus, Web of Science, ScienceDirect, and Google Scholar for studies published between 2010 and 2025. Eligible studies included in vivo trials evaluating plant-based nanoemulsions with measurable male reproductive outcomes. Data were pooled using a random-effects model. Mean differences (MD) and 95% confidence intervals (CI) were calculated for sperm concentration, sperm motility, and serum testosterone.</p>

                <p><strong>Results:</strong> Twenty-seven studies met the eligibility criteria. Meta-analysis showed a significant reduction in sperm concentration (MD: −42.7 million/mL; 95% CI: −55.2 to −30.3; p<0.001), sperm motility (MD: −28.4%; 95% CI: −36.9 to −19.8; p<0.01), and serum testosterone levels (MD: −1.42 ng/mL; 95% CI: −2.12 to −0.73; p<0.05). Histopathological findings consistently revealed degeneration of seminiferous tubules, Leydig cell suppression, reduced epithelial height, and impaired spermatogenesis. Nanoemulsion formulations improved bioavailability (2–8× increase) and reduced required doses compared to crude extracts. Toxicity was minimal and reversible in most studies.</p>

                <p><strong>Conclusion:</strong> Plant-based nanoemulsion formulations significantly enhance antifertility efficacy through improved testicular bioavailability, oxidative stress induction, and suppression of steroidogenesis. Their reversibility and safety profile highlight their potential use as non-surgical contraceptive options, particularly for canine population control programs. Further research in target veterinary species is recommended.</p>

                <div class="keywords-container">
                    <h4 class="mb-3">Keywords:</h4>
                    <span class="keyword-tag">Nanoemulsion</span>
                    <span class="keyword-tag">Antifertility</span>
                    <span class="keyword-tag">Phytochemicals</span>
                    <span class="keyword-tag">Spermatogenesis</span>
                    <span class="keyword-tag">Testosterone</span>
                    <span class="keyword-tag">Reproduction</span>
                </div>
            </div>
        </div>
    </section>

    <!-- Methods Section -->
    <section id="methods" class="section-padding">
        <div class="container">
            <h2 class="section-title fade-in">Methods</h2>
            <div class="card-modern fade-in">
                <div class="card-header-modern">
                    <i class="fas fa-microscope me-2"></i>
                    Research Methodology
                </div>
                <div class="card-body p-4">
                    <p class="lead">A PRISMA-guided systematic search was conducted across multiple databases for comprehensive literature review.</p>
                    
                    <div class="row mt-4">
                        <div class="col-md-6">
                            <h5><i class="fas fa-database me-2 text-primary"></i>Databases Searched:</h5>
                            <ul class="list-unstyled">
                                <li><i class="fas fa-check text-success me-2"></i>PubMed</li>
                                <li><i class="fas fa-check text-success me-2"></i>Scopus</li>
                                <li><i class="fas fa-check text-success me-2"></i>Web of Science</li>
                                <li><i class="fas fa-check text-success me-2"></i>ScienceDirect</li>
                                <li><i class="fas fa-check text-success me-2"></i>Google Scholar</li>
                            </ul>
                        </div>
                        <div class="col-md-6">
                            <h5><i class="fas fa-calendar-alt me-2 text-primary"></i>Study Period:</h5>
                            <p>Studies published between <strong>2010 and 2025</strong></p>
                            
                            <h5><i class="fas fa-filter me-2 text-primary"></i>Inclusion Criteria:</h5>
                            <ul class="list-unstyled">
                                <li><i class="fas fa-check text-success me-2"></i>In vivo trials</li>
                                <li><i class="fas fa-check text-success me-2"></i>Plant-based nanoemulsions</li>
                                <li><i class="fas fa-check text-success me-2"></i>Measurable reproductive outcomes</li>
                            </ul>
                        </div>
                    </div>

                    <div class="mt-4">
                        <h5><i class="fas fa-chart-line me-2 text-primary"></i>Statistical Analysis:</h5>
                        <p>Data were pooled using a random-effects model. Mean differences (MD) and 95% confidence intervals (CI) were calculated for sperm concentration, sperm motility, and serum testosterone.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Results Section -->
    <section id="results" class="section-padding bg-light">
        <div class="container">
            <h2 class="section-title fade-in">Results</h2>
            <div class="row">
                <div class="col-lg-8">
                    <div class="card-modern fade-in">
                        <div class="card-header-modern">
                            <i class="fas fa-chart-bar me-2"></i>
                            Study Overview
                        </div>
                        <div class="card-body p-4">
                            <p class="lead">Twenty-seven studies met the eligibility criteria for this comprehensive meta-analysis.</p>
                            
                            <h5 class="mt-4 mb-3">Key Findings:</h5>
                            <ul>
                                <li><strong>Histopathological Changes:</strong> Consistent degeneration of seminiferous tubules, Leydig cell suppression, reduced epithelial height, and impaired spermatogenesis.</li>
                                <li><strong>Bioavailability Enhancement:</strong> Nanoemulsion formulations showed 2–8× increase in bioavailability compared to crude extracts.</li>
                                <li><strong>Dose Reduction:</strong> Significantly reduced required doses compared to traditional crude extracts.</li>
                                <li><strong>Safety Profile:</strong> Toxicity was minimal and reversible in most studies.</li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="col-lg-4">
                    <div class="info-card fade-in">
                        <div class="info-label">
                            <i class="fas fa-file-medical-alt"></i>
                            Studies Analyzed
                        </div>
                        <div class="info-value display-4 text-primary">27</div>
                    </div>
                    
                    <div class="info-card fade-in">
                        <div class="info-label">
                            <i class="fas fa-microscope"></i>
                            Bioavailability Increase
                        </div>
                        <div class="info-value display-4 text-success">2-8×</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Meta-Analysis Results Section -->
    <section id="meta-analysis" class="section-padding">
        <div class="container">
            <h2 class="section-title fade-in">Meta-Analysis Results</h2>
            
            <!-- Summary Cards -->
            <div class="meta-results fade-in">
                <div class="result-card">
                    <div class="result-label">Sperm Concentration</div>
                    <div class="result-value">-42.7</div>
                    <div>million/mL</div>
                    <div class="result-ci">95% CI: -55.2 to -30.3</div>
                    <div class="text-danger fw-bold">p &lt; 0.001</div>
                </div>
                
                <div class="result-card">
                    <div class="result-label">Sperm Motility</div>
                    <div class="result-value">-28.4%</div>
                    <div>reduction</div>
                    <div class="result-ci">95% CI: -36.9 to -19.8</div>
                    <div class="text-danger fw-bold">p &lt; 0.01</div>
                </div>
                
                <div class="result-card">
                    <div class="result-label">Testosterone Levels</div>
                    <div class="result-value">-1.42</div>
                    <div>ng/mL</div>
                    <div class="result-ci">95% CI: -2.12 to -0.73</div>
                    <div class="text-danger fw-bold">p &lt; 0.05</div>
                </div>
            </div>

            <!-- Interactive Forest Plots -->
            <div class="row">
                <div class="col-lg-4 mb-4">
                    <div class="chart-container fade-in">
                        <h4 class="chart-title">Sperm Concentration</h4>
                        <canvas id="spermConcentrationChart"></canvas>
                    </div>
                </div>
                
                <div class="col-lg-4 mb-4">
                    <div class="chart-container fade-in">
                        <h4 class="chart-title">Sperm Motility</h4>
                        <canvas id="spermMotilityChart"></canvas>
                    </div>
                </div>
                
                <div class="col-lg-4 mb-4">
                    <div class="chart-container fade-in">
                        <h4 class="chart-title">Testosterone Levels</h4>
                        <canvas id="testosteroneChart"></canvas>
                    </div>
                </div>
            </div>

            <!-- Comprehensive Forest Plot -->
            <div class="chart-container fade-in">
                <h4 class="chart-title">Comprehensive Meta-Analysis Forest Plot</h4>
                <canvas id="forestPlotChart" style="height: 400px;"></canvas>
            </div>
        </div>
    </section>

    <!-- Discussion Section -->
    <section id="discussion" class="section-padding bg-light">
        <div class="container">
            <h2 class="section-title fade-in">Discussion</h2>
            <div class="row">
                <div class="col-lg-8">
                    <div class="card-modern fade-in">
                        <div class="card-header-modern">
                            <i class="fas fa-comments me-2"></i>
                            Research Implications
                        </div>
                        <div class="card-body p-4">
                            <p class="lead">This comprehensive meta-analysis demonstrates the significant potential of plant-based nanoemulsion formulations as effective antifertility agents.</p>
                            
                            <h5 class="mt-4 mb-3">Key Discussion Points:</h5>
                            
                            <div class="row">
                                <div class="col-md-6">
                                    <h6><i class="fas fa-dna me-2 text-primary"></i>Mechanistic Insights:</h6>
                                    <ul>
                                        <li>Enhanced testicular bioavailability</li>
                                        <li>Oxidative stress induction</li>
                                        <li>Suppression of steroidogenesis</li>
                                        <li>Direct impact on spermatogenesis</li>
                                    </ul>
                                </div>
                                
                                <div class="col-md-6">
                                    <h6><i class="fas fa-shield-alt me-2 text-primary"></i>Safety Profile:</h6>
                                    <ul>
                                        <li>Minimal toxicity observed</li>
                                        <li>Reversible effects</li>
                                        <li>Reduced dose requirements</li>
                                        <li>Better tolerability profile</li>
                                    </ul>
                                </div>
                            </div>

                            <h6 class="mt-4"><i class="fas fa-lightbulb me-2 text-primary"></i>Clinical Significance:</h6>
                            <p>The findings highlight the potential use of these formulations as non-surgical contraceptive options, particularly valuable for canine population control programs in veterinary medicine.</p>
                        </div>
                    </div>
                </div>
                
                <div class="col-lg-4">
                    <div class="card-modern fade-in">
                        <div class="card-header-modern">
                            <i class="fas fa-road me-2"></i>
                            Future Directions
                        </div>
                        <div class="card-body p-4">
                            <ul class="list-unstyled">
                                <li class="mb-2"><i class="fas fa-arrow-right me-2 text-success"></i>Target veterinary species research</li>
                                <li class="mb-2"><i class="fas fa-arrow-right me-2 text-success"></i>Long-term safety studies</li>
                                <li class="mb-2"><i class="fas fa-arrow-right me-2 text-success"></i>Optimization of formulations</li>
                                <li class="mb-2"><i class="fas fa-arrow-right me-2 text-success"></i>Clinical trial implementation</li>
                                <li class="mb-2"><i class="fas fa-arrow-right me-2 text-success"></i>Regulatory approval pathways</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Conclusion Section -->
    <section class="section-padding">
        <div class="container">
            <h2 class="section-title fade-in">Conclusion</h2>
            <div class="abstract-section fade-in">
                <p class="lead text-center mb-4">Plant-based nanoemulsion formulations significantly enhance antifertility efficacy through improved testicular bioavailability, oxidative stress induction, and suppression of steroidogenesis.</p>
                
                <div class="row mt-5">
                    <div class="col-md-4 text-center mb-4">
                        <i class="fas fa-check-circle fa-3x text-success mb-3"></i>
                        <h5>Enhanced Efficacy</h5>
                        <p>Significant improvements in reproductive parameter modifications with lower doses required.</p>
                    </div>
                    
                    <div class="col-md-4 text-center mb-4">
                        <i class="fas fa-shield-virus fa-3x text-primary mb-3"></i>
                        <h5>Safety Profile</h5>
                        <p>Minimal toxicity with reversible effects, making them suitable for practical applications.</p>
                    </div>
                    
                    <div class="col-md-4 text-center mb-4">
                        <i class="fas fa-paw fa-3x text-warning mb-3"></i>
                        <h5>Veterinary Applications</h5>
                        <p>Potential for canine population control programs as non-surgical contraceptive options.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact-section">
        <div class="container text-center">
            <h2 class="mb-4">Contact for Queries</h2>
            <p class="lead mb-4">For inquiries about this research or submission guidelines, please contact:</p>
            <a href="mailto:editor@veterinaryworld.org" class="contact-link">
                <i class="fas fa-envelope me-2"></i>
                editor@veterinaryworld.org
            </a>
            
            <div class="mt-5">
                <div class="author-card d-inline-block">
                    <h4>Author</h4>
                    <p class="mb-2">Harishkumar J. N.</p>
                    <a href="https://orcid.org/0009-0001-0254-2773" target="_blank" class="orcid-link">
                        <i class="fab fa-orcid fa-2x me-2"></i>
                        View ORCID Profile
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Scroll to Top Button -->
    <button class="btn-scroll-top" onclick="scrollToTop()">
        <i class="fas fa-arrow-up"></i>
    </button>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Scroll to top functionality
        function scrollToTop() {
            window.scrollTo({
                top: 0,
                behavior: 'smooth'
            });
        }

        // Show/hide scroll to top button
        window.addEventListener('scroll', function() {
            const scrollBtn = document.querySelector('.btn-scroll-top');
            if (window.scrollY > 300) {
                scrollBtn.classList.add('show');
            } else {
                scrollBtn.classList.remove('show');
            }

            // Update active navigation
            const sections = document.querySelectorAll('section[id]');
            const navLinks = document.querySelectorAll('.nav-link');
            
            let currentSection = '';
            sections.forEach(section => {
                const sectionTop = section.offsetTop - 100;
                if (window.scrollY >= sectionTop) {
                    currentSection = section.getAttribute('id');
                }
            });

            navLinks.forEach(link => {
                link.classList.remove('active');
                if (link.getAttribute('href') === '#' + currentSection) {
                    link.classList.add('active');
                }
            });
        });

        // Fade in animation on scroll
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, observerOptions);

        document.querySelectorAll('.fade-in').forEach(el => {
            observer.observe(el);
        });

        // Chart.js configurations for forest plots
        const chartOptions = {
            responsive: true,
            // maintainAspectRatio: false,
            plugins: {
                legend: {
                    display: false
                },
                tooltip: {
                    callbacks: {
                        title: function(tooltipItem) {
                            return 'Mean Difference';
                        },
                        label: function(tooltipItem) {
                            return `Effect Size: ${tooltipItem.formattedValue}`;
                        }
                    }
                }
            },
            scales: {
                x: {
                    beginAtZero: false,
                    title: {
                        display: true,
                        text: 'Effect Size'
                    },
                    grid: {
                        drawOnChartArea: true,
                        color: 'rgba(0,0,0,0.1)'
                    }
                },
                y: {
                    display: false
                }
            }
        };

        // Sperm Concentration Chart
        const spermConcentrationCtx = document.getElementById('spermConcentrationChart').getContext('2d');
        new Chart(spermConcentrationCtx, {
            type: 'scatter',
            data: {
                datasets: [{
                    label: 'Effect Size',
                    data: [{x: -42.7, y: 1}],
                    backgroundColor: '#2c5530',
                    borderColor: '#2c5530',
                    pointRadius: 8,
                    pointHoverRadius: 12
                }, {
                    label: 'Confidence Interval',
                    data: [{x: -55.2, y: 1}, {x: -30.3, y: 1}],
                    backgroundColor: 'transparent',
                    borderColor: '#7cb342',
                    borderWidth: 3,
                    pointRadius: 0,
                    showLine: true,
                    tension: 0
                }]
            },
            options: {
                ...chartOptions,
                scales: {
                    ...chartOptions.scales,
                    x: {
                        ...chartOptions.scales.x,
                        title: {
                            ...chartOptions.scales.x.title,
                            text: 'Mean Difference (million/mL)'
                        }
                    }
                }
            }
        });

        // Sperm Motility Chart
        const spermMotilityCtx = document.getElementById('spermMotilityChart').getContext('2d');
        new Chart(spermMotilityCtx, {
            type: 'scatter',
            data: {
                datasets: [{
                    label: 'Effect Size',
                    data: [{x: -28.4, y: 1}],
                    backgroundColor: '#4a7c59',
                    borderColor: '#4a7c59',
                    pointRadius: 8,
                    pointHoverRadius: 12
                }, {
                    label: 'Confidence Interval',
                    data: [{x: -36.9, y: 1}, {x: -19.8, y: 1}],
                    backgroundColor: 'transparent',
                    borderColor: '#7cb342',
                    borderWidth: 3,
                    pointRadius: 0,
                    showLine: true,
                    tension: 0
                }]
            },
            options: {
                ...chartOptions,
                scales: {
                    ...chartOptions.scales,
                    x: {
                        ...chartOptions.scales.x,
                        title: {
                            ...chartOptions.scales.x.title,
                            text: 'Mean Difference (%)'
                        }
                    }
                }
            }
        });

        // Testosterone Chart
        const testosteroneCtx = document.getElementById('testosteroneChart').getContext('2d');
        new Chart(testosteroneCtx, {
            type: 'scatter',
            data: {
                datasets: [{
                    label: 'Effect Size',
                    data: [{x: -1.42, y: 1}],
                    backgroundColor: '#7cb342',
                    borderColor: '#7cb342',
                    pointRadius: 8,
                    pointHoverRadius: 12
                }, {
                    label: 'Confidence Interval',
                    data: [{x: -2.12, y: 1}, {x: -0.73, y: 1}],
                    backgroundColor: 'transparent',
                    borderColor: '#4a7c59',
                    borderWidth: 3,
                    pointRadius: 0,
                    showLine: true,
                    tension: 0
                }]
            },
            options: {
                ...chartOptions,
                scales: {
                    ...chartOptions.scales,
                    x: {
                        ...chartOptions.scales.x,
                        title: {
                            ...chartOptions.scales.x.title,
                            text: 'Mean Difference (ng/mL)'
                        }
                    }
                }
            }
        });

        // Comprehensive Forest Plot
        const forestPlotCtx = document.getElementById('forestPlotChart').getContext('2d');
        new Chart(forestPlotCtx, {
            type: 'scatter',
            data: {
                datasets: [{
                    label: 'Sperm Concentration',
                    data: [{x: -42.7, y: 3}],
                    backgroundColor: '#2c5530',
                    borderColor: '#2c5530',
                    pointRadius: 10,
                    pointHoverRadius: 15
                }, {
                    label: 'Sperm Motility',
                    data: [{x: -28.4, y: 2}],
                    backgroundColor: '#4a7c59',
                    borderColor: '#4a7c59',
                    pointRadius: 10,
                    pointHoverRadius: 15
                }, {
                    label: 'Testosterone',
                    data: [{x: -1.42, y: 1}],
                    backgroundColor: '#7cb342',
                    borderColor: '#7cb342',
                    pointRadius: 10,
                    pointHoverRadius: 15
                }]
            },
            options: {
                responsive: true,
                // maintainAspectRatio: false,
                plugins: {
                    legend: {
                        display: true,
                        position: 'top'
                    },
                    tooltip: {
                        callbacks: {
                            title: function(tooltipItem) {
                                const labels = ['Testosterone', 'Sperm Motility', 'Sperm Concentration'];
                                return labels[tooltipItem[0].parsed.y - 1];
                            },
                            label: function(tooltipItem) {
                                const values = ['-1.42 ng/mL', '-28.4%', '-42.7 million/mL'];
                                const cis = ['(-2.12 to -0.73)', '(-36.9 to -19.8)', '(-55.2 to -30.3)'];
                                const ps = ['p<0.05', 'p<0.01', 'p<0.001'];
                                const idx = tooltipItem.parsed.y - 1;
                                return [`Effect Size: ${values[idx]}`, `95% CI: ${cis[idx]}`, `${ps[idx]}`];
                            }
                        }
                    }
                },
                scales: {
                    x: {
                        title: {
                            display: true,
                            text: 'Effect Size (Favors Treatment)',
                            font: {
                                size: 14,
                                weight: 'bold'
                            }
                        },
                        grid: {
                            drawOnChartArea: true,
                            color: 'rgba(0,0,0,0.1)'
                        }
                    },
                    y: {
                        min: 0.5,
                        max: 3.5,
                        ticks: {
                            stepSize: 1,
                            callback: function(value) {
                                const labels = ['', 'Testosterone', 'Sperm Motility', 'Sperm Concentration'];
                                return labels[value] || '';
                            }
                        },
                        grid: {
                            drawOnChartArea: false
                        }
                    }
                }
            }
        });
    </script>
</body>
</html>
