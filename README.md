# Kyvernitis Resume
A batteries included LaTeX Resume Template specifically designed for software developers, especially new grads. This comprehensive template is perfect for creating compact and impressive resumes. With its single-column layout, you can create a concise single-page resume that showcases your skills effectively, or a bit more elaborate multi page ones if you like!

## Key Features
- **Versatile Format:** This template is not limited to a single page; you can easily expand it to multiple pages if needed. However, it is primarily optimized for a single-page layout.
- **Social Account Integration:** You have the flexibility to include up to 6 social accounts in your resume heading. These can include **LinkedIn**, **GitHub**, **Facebook**, **Email**, **Website**, **Current Address**, **Nationality**, and **Phone number**. You just have to put your username, it will link to the respective account **automatically**.
- **Dynamic Heading:** You can also add your job title using the \jobtitle command, and the heading will adjust accordingly to display it prominently.
- **Intuitive:** Instead of creating new separate commands, I reused the section and subsection command, so that you can write a resume *blazingly fast*. Even though I am overriding those commands, the PDF generated will still have a table of content, for easier navigation in case you are planning to create a large CV.

## Example
![image](https://github.com/aretrosen/kyvernetes-resume/assets/125266845/c67e3edc-907f-46da-91fb-6dfc191ca00e)


## Usage
```tex
\documentclass[]{kyvernitis-resume}

% Put you name here
\fullname{your-name}
\jobtitle{your-job-title} %Optional job title

\begin{document}

% This is the resume header. For LinkedIn, GitHub, Email, Facebook, and Website, it will automatically link it the respective accounts.
\resumeheader{\linkedin{your-linkedin-username}}{...}{...}{...}{...}{...} % Don't keep the dots, just put additional social accounts. Upto 6 supported.

% Now put any number of sections. 
\begin{section}{your-section-name}

  % Lets make a subsection with bulletted items.
  \begin{subsection}{your-subsection-name}{your-subsection-description}{time-period}{location}
    \item{...}          % This will create an item in plaintext
    \italicitem{...}    % As you can guess, this will create an item with italic text
    \bolditem{...}      % You can probably guess it, right?
  \end{subsection}
  
  % Now let's make a subsection with no bullets
  \begin{subsectionnobullet}{your-subsection-name}{your-subsection-description}{time-period}{location}
    % Put whatever you like below, as above
    ...
  \end{subsectionnobullet}
  
  % Now lets make a section which acts like a table.
  \sectiontable{your-section-table-name}{
    \entry{your-entry-name}{details-about-your-entry}
  }
  
\end{section}

\end{document}
```
That's it! This is as easy as it gets. Additionally, you don't have to think of margins, formtting etc. every time, and don't have to reach for your mouse for the same. Just write it, generate a pdf, and you are done!

## How to use this template in Overleaf?
Just download the zip file, and import the zip file in your Overleaf account. And it's done!
