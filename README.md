# Resume
- %% It may be distributed and/or modified under the
- %% conditions of the LaTeX Project Public License, either version 1.3
- %% of this license or (at your option) any later version.
- %% The latest version of this license is in
- %%    http://www.latex-project.org/lppl.txt
- %% and version 1.3 or later is part of all distributions of LaTeX
- %% version 2003/12/01 or later.
%%%%%%%%%%%%%%%%

%% Use the "normalphoto" option if you want a normal photo instead of cropped to a circle
% \documentclass[10pt,a4paper,normalphoto]{altacv}

\documentclass[10pt,a4paper,ragged2e,withhyper]{altacv}
%% AltaCV uses the fontawesome5 package.
%% See http://texdoc.net/pkg/fontawesome5 for full list of symbols.

% Change the page layout if you need to
\geometry{left=1.25cm,right=1.25cm,top=1.5cm,bottom=1.5cm,columnsep=1.2cm}

% The paracol package lets you typeset columns of text in parallel
\usepackage{paracol}


% Change the font if you want to, depending on whether
% you're using pdflatex or xelatex/lualatex
% WHEN COMPILING WITH XELATEX PLEASE USE
% xelatex -shell-escape -output-driver="xdvipdfmx -z 0" mmayer.tex
\ifxetexorluatex
  % If using xelatex or lualatex:
  \setmainfont{Lato}
\else
  % If using pdflatex:
  \usepackage[default]{lato}
\fi

% Change the colours if you want to
\definecolor{VividPurple}{HTML}{3E0097}
\definecolor{SlateGrey}{HTML}{2E2E2E}
\definecolor{LightGrey}{HTML}{666666}
% \colorlet{name}{black}
% \colorlet{tagline}{PastelRed}
\colorlet{heading}{VividPurple}
\colorlet{headingrule}{VividPurple}
% \colorlet{subheading}{PastelRed}
\colorlet{accent}{VividPurple}
\colorlet{emphasis}{SlateGrey}
\colorlet{body}{LightGrey}

% Change some fonts, if necessary
% \renewcommand{\namefont}{\Huge\rmfamily\bfseries}
% \renewcommand{\personalinfofont}{\footnotesize}
% \renewcommand{\cvsectionfont}{\LARGE\rmfamily\bfseries}
% \renewcommand{\cvsubsectionfont}{\large\bfseries}

% Change the bullets for itemize and rating marker
% for \cvskill if you want to
\renewcommand{\cvItemMarker}{{\small\textbullet}}
\renewcommand{\cvRatingMarker}{\faCircle}
% ...and the markers for the date/location for \cvevent
% \renewcommand{\cvDateMarker}{\faCalendar*[regular]}
% \renewcommand{\cvLocationMarker}{\faMapMarker*}


% If your CV/résumé is in a language other than English,
% then you probably want to change these so that when you
% copy-paste from the PDF or run pdftotext, the location
% and date marker icons for \cvevent will paste as correct
% translations. For example Spanish:
% \renewcommand{\locationname}{Ubicación}
% \renewcommand{\datename}{Fecha}


%% Use (and optionally edit if necessary) this .tex if you
%% want to use an author-year reference style like APA(6)
%% for your publication list
% \input{pubs-authoryear.tex}

%% Use (and optionally edit if necessary) this .tex if you
%% want an originally numerical reference style like IEEE
%% for your publication list
\input{pubs-num.tex}

%% sample.bib contains your publications
\addbibresource{sample.bib}

\begin{document}
\name{THANMAI BALABHADRA}
% Cropped to square from https://en.wikipedia.org/wiki/Marissa_Mayer#/media/File:Marissa_Mayer_May_2014_(cropped).jpg, CC-BY 2.0
%% You can add multiple photos on the left or right
\photoR{2.5cm}{img.jpg}
% photoL{2cm}{Yacht_High,Suitcase_High}
\personalinfo{%
  % Not all of these are required!
  % You can add your own with \printinfo{symbol}{detail}
  \email{thanmai.balabhadra@sasi.ac.in}
  \phone{9490859733}
  \mailaddress{Tanuku,Andhrapradesh,India}
  \linkedin{thanmai-balabhadra-135879277}
\github{ThanmaiBalabhadra}
\homepage {thanmaiportfolio.netlify.app}
  % I'm just making this up though.
% \orcid{0000-0000-0000-0000} % Obviously making this up too.
  %% You can add your own arbitrary detail with
  %% \printinfo{symbol}{detail}[optional hyperlink prefix]
  % \printinfo{\faPaw}{Hey ho!}
  %% Or you can declare your own field with
  %% \NewInfoFiled{fieldname}{symbol}[optional hyperlink prefix] and use it:
  % \NewInfoField{gitlab}{\faGitlab}[https://gitlab.com/]
  % \gitlab{your_id}
	%%
  %% For services and platforms like Mastodon where there isn't a
  %% straightforward relation between the user ID/nickname and the hyperlink,
  %% you can use \printinfo directly e.g.
  % \printinfo{\faMastodon}{@username@instace}[https://instance.url/@username]
  %% But if you absolutely want to create new dedicated info fields for
  %% such platforms, then use \NewInfoField* with a star:
  % \NewInfoField*{mastodon}{\faMastodon}
  %% then you can use \mastodon, with TWO arguments where the 2nd argument is
  %% the full hyperlink.
  % \mastodon{@username@instance}{https://instance.url/@username}
}

\makecvheader

%% Depending on your tastes, you may want to make fonts of itemize environments slightly smaller
\AtBeginEnvironment{itemize}{\small}

%% Set the left/right column width ratio to 6:4.
\columnratio{0.6}

% Start a 2-column paracol. Both the left and right columns will automatically
% break across pages if things get too long.
\begin{paracol}{2}
\cvsection{internship experience}
\cvevent{MERN Stack}{EXCELR}{jun 2024 -- jul 2024}{Remote}
\begin{itemize}
\item {  
A short-term internship focused on the MERN stack (MongoDB, Express.js, React, and Node.js) typically involves hands-on experience in developing web applications using these technologies.} 
 \item \cvevent{}{\href{https://drive.google.com/file/d/1JZ7ttl1PtUDAB3K2lLvLMEv93uBjAPgD/view?usp=sharing}{View Certificate}}{}{}
\cvtag{MongoDB}
\cvtag{Express.js}
\cvtag{React.js}
\cvtag{Node.js}
\end{itemize}
\divider
\cvevent{Web Development internship}{CodSoft}{Dec 2023 --jan 2024}{Remote}
\begin{itemize}
\item  
Web development involves creating, building, and maintaining websites and web applications, covering both front-end (user interface) and back-end (server-side) aspects to ensure functionality, security, and performance.\\
\item \cvevent{}{\href{https://drive.google.com/file/d/1LdNRDWxdIq5rAo_-CYYFLcnr6bN-8o3O/view?usp=drivesdk}{View Certificate}}{}{}
\cvtag{HTML}
\cvtag{CSS}
\cvtag{JavaScript}
\end{itemize}
\divider

\cvsection{PROJECTS}
\cvevent{\textbf{LingoReplica}}{}{}{}{
\begin{itemize}
    \item LingoReplica is an advanced web app that uses the Google Translate API for multilingual text translation. It features a streamlined interface with language selection, document upload, character count tracking, and optional dark mode.
    \item \cvevent{}{\href{https://sweet-kitsune-11c60a.netlify.app/}{Live Demo}, \href{https://github.com/ThanmaiBalabhadra/Google-Translate-Clone.git}{GitHub Repo}}{}{}


    
\cvtag{Html,CSS}
\cvtag{JavaScript}
\cvtag{CSS Animations}
\cvtag{Netlify}
    \end{itemize}
    \divider
\cvevent{\textbf{Amazon-Clone}}{}{}{}{
\begin{itemize}
    \item A frontend clone of E-commerce website of Amazon. This is created using HTML,CSS and Vanilla Javascript. The page is created for big screens i.e, laptops, PCs only.
    \item \cvevent{}{\href{https://spectacular-dasik-70af80.netlify.app/}{Live Demo}, \href{https://github.com/ThanmaiBalabhadra/Amazon-Clone.git}{GitHub Repo}}{}{}




\cvtag{Html}
\cvtag{CSS}
\cvtag{JavaScript}


\end{itemize}

\divider


\cvevent{\textbf{VocalizeIt}}{}{}{}{
\begin{itemize}
    \item Developed text-to-speech functionality using HTML, CSS, and JavaScript with the Web Speech API, enabling the browser to convert text into spoken audio and enhance user accessibility and interaction.
    \item \cvevent{}{\href{https://frabjous-faloodeh-ec7e1e.netlify.app/}{Live Demo}, \href{https://github.com/ThanmaiBalabhadra/Text-to-speech.git}{GitHub Repo}}{}{}
    

\cvtag{Html}
\cvtag{CSS}
\cvtag{JavaScript}

\end{itemize}

% use ONLY \newpage if you want to force a page break for
% ONLY the currentc column
\newpage


\printbibliography[heading=pubtype,title={\printinfo{\faUsers}{Conference Proceedings}},type=inproceedings]

%% Switch to the right column. This will now automatically move to the second
%% page if the content is too long.
\switchcolumn

\cvsection{ACHIEVEMENTS}

\cvachievement{\faTrophy}{Awarded}{Awarded State 1st in Aryabhatta Olympiad }

\divider

\cvachievement{\faUsers}{Team-Lead}{Awarded 1st Place Champion of the District Level Badminton}
\smallskip

\cvsection{CERTIFICATIONS}
\begin{itemize}
     \item {\href{https://www.hackerrank.com/certificates/77336fc6267c}{Python certification from HackerRank \textbf{-VIEW}}}
        \item {\href{https://drive.google.com/file/d/1LtmerEAqO5XuF_DFddQq2FXYQ0B2F5yc/view?usp=drivesdk}{HTML5 and CSS Fundamentals Certification from EdX\textbf{-VIEW}}}
        \item {\href{https://drive.google.com/file/d/1Lq4mtKgAivM8hPy6aVj1wAsZNIT79pHs/view?usp=drivesdk}{Linux Certification (RH104) from Red Hat \textbf{-VIEW}}}
    
\end{itemize}

\cvsection{EDUCATION}
\cvevent{B.TECH CST\ }{Sasi Institute of Technology and Engineering – 8.92 CGPA}{ 2021-2025} {Tadepalligudem}

\divider

\cvevent{INTERMEDIATE}{Smt.Annapurna Junior College – 10 CGPA}{2019-2021}{Velivennu}

\divider

\cvevent{SSC\ }{Smt. Annapurna Vidya Nikethan – 10 CGPA}{ 2018-2019} {Velivennu}
\divider

\cvsection{Skills}
\begin{itemize}
    \item \textbf{Frontend :  } 
    \cvtag{HTML} \cvtag{CSS} \cvtag{BootStrap} \cvtag{JavaScript} \cvtag{React.js}
    \item \textbf{Backend : }
    \cvtag{Node.js}
     \item \textbf{Programming Languages : } \cvtag{Python} \cvtag{Java} \cvtag{C}
    \item \textbf{Databases: } \cvtag{MySQL} \cvtag{MongoDB}
    \item \textbf{OS : }
    \cvtag{Linux,Windows}
     \item \textbf{Version Control : } 
    \cvtag{Git}
     \item \textbf{IDEs and Tools : } 
  \cvtag{Visual Studio Code}  \cvtag{Docker} \cvtag{Jenkins} \cvtag{Netlify}
    
\end{itemize}

\newpage

\end{paracol}

\end{document}
