html: Presentation.ipynb
	jupyter nbconvert --to slides Presentation.ipynb --template=./cwi_template
	mv Presentation.slides.html html/Presentation.html
	cp -r figures ./html
website: html
	ghp-import --no-jekyll --no-history --push --force html/
