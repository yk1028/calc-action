# calc-action
``` yaml
jobs:
  calculate:
    runs-on: ubuntu-latest
    steps:
      - uses: yk1028/yk1028-calc-action@v0.0.1
        with:
          x: 12
          y: 3
      - name: print results
        run: |
          echo "x + y = ${{ steps.calc.outputs.plus }}"
          echo "x - y = ${{ steps.calc.outputs.minus }}"
          echo "x * y = ${{ steps.calc.outputs.multiply }}"
          echo "x / y = ${{ steps.calc.outputs.divide }}"
```
