# plant-detection
\documentclass[11pt,aspectratio=169,notes,mathserif]{beamer}

\usepackage[utf8]{inputenc}
\usepackage[T1]{fontenc}
\usefonttheme{serif}
\usepackage[english]{babel}
\usetheme{Madrid}
\usepackage{graphicx}
\usepackage{bm}
\usepackage{ragged2e}
\usepackage{amsmath,amsfonts,amssymb}
\usepackage{lmodern}
\usepackage{tikz}
\usepackage{etoolbox}

\setbeamertemplate{caption}[numbered]
\setbeamertemplate{frametitle continuation}[from second][\textbf{(contd..)}]

\addtobeamertemplate{frametitle}{}{%
  \begin{tikzpicture}[remember picture,overlay]
    \fill (14.5,0.6) circle (.8cm);
    \clip (14.5,0.5) circle (.75cm);
    \node at (14.5,0.6) {\includegraphics[width=0.95cm]{bvrit.JPG}};
\end{tikzpicture}}

\renewcommand{\raggedright}{\justifying}
\apptocmd{\frame}{}{\justifying}{}

%------------------------------------------------

\title[\textbf{Department of CSE}]{{\textbf{Plant Disease Detection Using AI}}}

\author[Team No:8]{%
\begin{columns}
\column{.2\linewidth}\centering Indhu\\541
\column{.2\linewidth}\centering Tanvi\\542
\column{.2\linewidth}\centering Nandini\\543

\end{columns}
}

\institute{
Under the Guidance of \\
\textbf{ Dr.C.Rajeev} \\
Assistant Professor, Dept of C.S.E \\
BVRIT Hyderabad College of Engineering for Women
}

\date{April 23, 2026}

\logo{\includegraphics[width=1cm]{wise.png}}

%------------------------------------------------
\begin{document}

% Title Page
\begin{frame}
\titlepage
\end{frame}

% Table of Contents
\begin{frame}{Table of Content}
\tableofcontents
\end{frame}

%------------------------------------------------
\section{Abstract}

\begin{frame}{Abstract}
Plant diseases are a major challenge to agricultural productivity and food security. Traditional detection methods rely on manual inspection, which is time-consuming and prone to errors.

This project presents an AI-based plant disease detection system using deep learning techniques, especially Convolutional Neural Networks (CNN). The system analyzes leaf images to detect diseases accurately.

It provides fast, reliable, and automated disease detection, reducing dependency on experts. The system can be deployed as a web or mobile application for real-time use by farmers.
\end{frame}

%------------------------------------------------
\section{Introduction}

\begin{frame}{Introduction}
Agriculture plays a vital role in the economy, but plant diseases reduce crop yield and quality.

Traditional methods depend on manual inspection, which is slow and unreliable. Farmers often face difficulty in early detection.

This project introduces an AI-based system that detects plant diseases automatically using image processing and deep learning, helping farmers take timely action.
\end{frame}

%------------------------------------------------
\section{Literature Review}

\begin{frame}{Literature Review Summary}

\begin{table}[htbp]
\centering
\renewcommand{\arraystretch}{1.2}
\setlength{\tabcolsep}{4pt}
\begin{tabular}{|p{3cm}|p{2.5cm}|p{2.5cm}|p{2.5cm}|p{2.5cm}|}
\hline
Aspect & Traditional & ML Models & DL Models & Our System \\
\hline
Accuracy & Low & Medium & High & High \\
\hline
Speed & Slow & Medium & Fast & Fast \\
\hline
Automation & No & Partial & Yes & Yes \\
\hline
Scalability & Low & Medium & High & High \\
\hline
\end{tabular}
\caption{Comparison of Disease Detection Methods}
\end{table}

\end{frame}

%------------------------------------------------
\section{Technology Stack}

\begin{frame}{Technology Stack}

\begin{itemize}
\item Programming Language: Python
\item Frameworks: TensorFlow, Keras
\item Image Processing: OpenCV
\item Algorithm: CNN (Convolutional Neural Network)
\item Dataset: PlantVillage Dataset
\item Visualization: Matplotlib
\item Deployment: Web / Mobile Application
\end{itemize}

\end{frame}

%------------------------------------------------
\section{Packages}

\begin{frame}{Libraries Used}

\begin{itemize}
\item TensorFlow
\item Keras
\item OpenCV
\item NumPy
\item Pandas
\item Matplotlib
\end{itemize}

\end{frame}

%------------------------------------------------
\section{System Modules}

\begin{frame}{System Modules}

\begin{itemize}
\item User Interface Module – Upload images and view results
\item Image Processing Module – Resize, normalize, filter images
\item Disease Detection Engine – CNN-based classification
\item Explainability Module – Highlights affected regions
\item Analytics Module – Stores and tracks results
\end{itemize}

\end{frame}

%------------------------------------------------
\section{Methodology}

\begin{frame}{Methodology}

\begin{enumerate}
\item Image Input from user
\item Image Preprocessing using OpenCV
\item Feature Extraction
\item CNN Model Prediction
\item Disease Classification Output
\end{enumerate}

\end{frame}

%------------------------------------------------
\section{Results}

\begin{frame}{Results}

\begin{itemize}
\item High accuracy in disease detection
\item Fast and real-time prediction
\item Clear visualization of affected areas
\item User-friendly interface
\end{itemize}

\end{frame}

%------------------------------------------------
\section{Conclusion}

\begin{frame}{Conclusion}

The AI-based plant disease detection system provides an efficient and accurate solution for identifying plant diseases.

It reduces manual effort and enables early detection. The use of CNN improves prediction accuracy, and the explainability feature enhances user trust.

Overall, the system helps improve crop productivity and supports smart agriculture.

\end{frame}

%------------------------------------------------
\section{References}

\begin{frame}{References}
\footnotesize

\begin{itemize}
\item Alex Krizhevsky - ImageNet Classification
\item Kaiming He - ResNet Paper
\item Grad-CAM Research Paper
\item TensorFlow Documentation
\item Keras Documentation
\end{itemize}

\end{frame}

%------------------------------------------------
\end{document}
