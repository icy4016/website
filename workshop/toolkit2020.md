---
title: Advanced MEG/EEG toolkit at the Donders
---

# Advanced MEG/EEG toolkit at the Donders

From 20-24 April 2020 we will again host the “Advanced MEG/EEG toolkit”. Although initially scheduled to take place at the Donders Institute in Nijmegen, the COVID-19 situation made that impossible. We are instead hosting it online.

Organizers: Robert Oostenveld and Jan-Mathijs Schoffelen, with the help of many colleagues from the Donders and abroad.

This toolkit course will teach you advanced MEG and EEG data analysis skills. Preprocessing, frequency analysis, source reconstruction and various statistical methods will be covered. Furthermore, there will be a lot of attention to best practices for reproducible analysis and to Open Science. The toolkit will consist of a number of lectures, followed by hands-on sessions in which you will be tutored through the complete analysis of a MEG and EEG data set using the FieldTrip toolbox.

Even though we host the toolkit course online, we can only host a limited number of participants. To achieve good interaction between lecturers and participants - and especially tutors and participants in the hands-on sessions -  we have to limit the online attendance. Where possible we will record online events and share those afterwards.

We're pleased to have the following colleagues as our tutors:
* [Ashley Lewis](https://www.ru.nl/english/people/lewis-a/)
* [Christoph Huber-Huber](http://christoph.huber-huber.at/)
* [Eleanor Huizeling](https://www.mpi.nl/people/huizeling-eleanor)
* [Elie Rassi](https://www.ru.nl/english/people/el-rassi-e/)
* [Eric Maris](https://www.ru.nl/english/people/maris-e/)
* [Frederik Weber](https://www.ru.nl/english/people/weber-f/)
* [Hesham ElShafeh](https://twitter.com/heshamelshaf3i)
* [Jan-Mathijs Schoffelen](https://www.ru.nl/english/people/schoffelen-j/)
* [Joey Zhou](https://www.ru.nl/english/people/zhou-y/)
* [Johannes Algermissen](https://www.ru.nl/english/people/algermissen-j/)
* [Kristijan Armeni](https://www.ru.nl/english/people/armeni-k/)
* [Lau Moller Andersen](https://www.laumollerandersen.org/)
* [Martin Dresler](https://www.ru.nl/english/people/dresler-m/)
* [Mats van Es](https://www.ru.nl/english/people/es-m-van/)
* [Mikkel Vinding](https://natmeg.se/staff/mikkel%20vinding.html)
* [Robert Oostenveld](https://robertoostenveld.nl/research/)
* [Sophie Arana](https://www.mpi.nl/people/arana-sophie)
* [Stephen Whitmarch](https://stephenwhitmarsh.com/)
* [Vitoria Piai](http://vitoriapiai.ruhosting.nl/)
* [Xiaochen Zheng](https://www.ru.nl/english/people/zheng-x/)

## Test your MATLAB and FieldTrip installation

Prior to the hands-on sessions, we want you to provide us with some information with respect to the computational setup you have on your end. This is needed for us to anticipate (and ideally fix) any restrictions on your end. Also, it is needed to avoid a lot of time to be spent during the first session to get everybody up-and-running.

Therefore, please start MATLAB on your computer, copy-and-paste the code below into the MATLAB command line, and make a screenshot of the output you get on your screen. Please upload this screenshot in your personal hands-on notes google document so that we can check.

    fprintf('################################################################\n');
    fprintf('computer: %s\n', computer);
    ver('MATLAB');

    [ftver, ftpath] = ft_version;
    fprintf('FieldTrip path is at: %s\n', ftpath);
    fprintf('FieldTrip version is: %s\n', ftver);
    fprintf('ttest is:        %s\n', which('ttest'))
    fprintf('imdilate is:     %s\n', which('imdilate'));
    fprintf('dpss is:         %s\n', which('dpss'));
    fprintf('fminunc is:      %s\n', which('fminunc'));
    fprintf('ft_read_data is: %s\n', which('ft_read_data'));
    fprintf('runica is:       %s\n', which('runica'));  % should not be found yet, or the fieldtrip version
    fprintf('spm is:          %s\n', which('spm'));     % should not be found yet, or the fieldtrip version
    fprintf('################################################################\n');

If you get an error that says `Undefined function or variable 'ft_version'.` please add FieldTrip to the MATLAB path and try again. See [here](/faq/should_i_add_fieldtrip_with_all_subdirectories_to_my_matlab_path/) for more information about adding FieldTrip to the MATLAB search path.
