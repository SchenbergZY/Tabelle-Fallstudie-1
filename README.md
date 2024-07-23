# Difference from https://github.com/quadriga-dk/Tabelle-Fallstudie-1:

## 1. Editing .github/workflow/

    Adding R installation after python setup announcement.
    `
    - name: Set up R 
      uses: r-lib/actions/setup-r@v2
        
    - name: Install IRkernel
      run: |
        Rscript -e "install.packages('IRkernel')"
    `

    Register IRkernel after pip install requirments.
    `
    - name: Register IRkernel
      run: |
        Rscript -e "IRkernel::installspec()"
    `

## 2. 
    

