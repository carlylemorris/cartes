# Cartes Excel Add-In
An Excel Add-In for creating the cartesian product of multiple cell ranges, enabling multi-dimensional loop unrolling.

## Installation

### Download the `.xlam` File:
Download the `CARTES.xlam` file from this repository.

### Load the Add-In:
1. Open Excel and go to `File > Options > Add-Ins`.
2. In the `Manage:` dropdown at the bottom, select `Excel Add-ins` and click `Go...`.
3. Click `Browse...` and locate the downloaded `Cartes.xlam` file.
4. Check the box next to the add-in to enable it, then click `OK`.

## Usage

### Generating the Cartesian Product
To generate the Cartesian product of two or more ranges:

**Identify Input Ranges**

Input Ranges can be rows, columns or both

**Enter the Formula:**

Example with ranges `A2:A10` and `B1:Z1`:

```excel
=CARTES(A2:A10, B1:Z1)
```

Confirm as an array formula (Ctrl+Shift+Enter) if needed.

### Transpose Output (Optional)
If each combination should be in columns instead of rows:

```excel
=TRANSPOSE(CARTES(A2:A10, B1:Z1))
```


