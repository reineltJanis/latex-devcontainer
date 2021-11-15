FROM sharelatex/sharelatex

RUN tlmgr update --self --force --all && \
tlmgr install texliveonfly helvetic epstopdf times latexindent latexmk sectsty

RUN cpan -i YAML::Tiny File::HomeDir Unicode::GCString