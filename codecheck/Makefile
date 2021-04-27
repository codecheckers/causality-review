all: codecheck.pdf

codecheck.pdf: codecheck.ipynb codecheck_logo.png nbconvert_template.tex.j2 ../codecheck.yml outputs/extracted_S1_paper.png outputs/extracted_S1_repo.png outputs/conda_list.txt outputs/figures_err.txt outputs/figures/computational-times.txt outputs/figures/corr_plots.eps outputs/figures/corr_plots.pdf outputs/figures/corr_transforms_plots.eps outputs/figures/corr_transforms_plots.pdf outputs/figures/hb_figure1.eps outputs/figures/hb_figure1.pdf outputs/figures/hb_figure2.eps outputs/figures/hb_figure2.pdf outputs/figures/hu_figure.eps outputs/figures/hu_figure.pdf outputs/figures/lp_figure.eps outputs/figures/lp_figure.pdf outputs/figures/ul_figure.eps outputs/figures/ul_figure.pdf outputs/figures/ul_gaussian_figure.eps outputs/figures/ul_gaussian_figure.pdf outputs/figures/ul_missing_figure.eps outputs/figures/ul_missing_figure.pdf outputs/figures/ul_rounding_figure.eps outputs/figures/ul_rounding_figure.pdf outputs/figures/ul_scaling_figure.eps outputs/figures/ul_scaling_figure.pdf outputs/figures/ul-transforms.txt outputs/simulation-data/lp_time.csv outputs/simulation-data/lp_values.csv
	jupyter nbconvert --to pdf --no-input --no-prompt --execute --LatexExporter.template_file nbconvert_template.tex.j2 codecheck.ipynb

.PHONY: all clean

clean:
	rm -f codecheck.pdf
