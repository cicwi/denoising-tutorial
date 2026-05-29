html: Presentation.ipynb
	jupyter nbconvert --to slides Presentation.ipynb --template=./cwi_template
	mv Presentation.slides.html html/Presentation.html
	cp cwi_template/static/cwi_logo.png cwi_template/static/red_32.png html/
	cp -r figures ./html
website: html
	ghp-import --no-jekyll --no-history --push --force html/
