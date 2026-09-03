.PHONY: all en zh clean

all: en zh

en: resume_agent_focus_en.pdf

zh: resume_agent_focus_zh.pdf

resume_agent_focus_en.pdf: resume_agent_focus_en.tex
	latexmk -pdf -interaction=nonstopmode -halt-on-error $<

resume_agent_focus_zh.pdf: resume_agent_focus_zh.tex
	latexmk -xelatex -interaction=nonstopmode -halt-on-error $<

clean:
	latexmk -c resume_agent_focus_en.tex
	latexmk -c resume_agent_focus_zh.tex
