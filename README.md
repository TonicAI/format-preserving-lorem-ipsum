# Format Preserving Lorem Ipsum Text Generation

Format preserving Lorem Ipsum text generator replaces text in a source text with Lorem Ipsum, while
preserving some Unicode punctiontion, all Unicode control characters (e.g. newline and tab), and
replacing Unicode numbers with random digits between 0 and 9.

## Requirements

Python 3.5+

## Usage

Masking a file.

```
$ python mask.py <input_file.py>
```

Masking an input stream.

```
$ cat <input_file> | python mask.py
```
