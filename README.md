# Format Preserving Lorem Ipsum Text Generation

![](demo.gif)

Format preserving Lorem Ipsum text generator replaces a source text with Lorem Ipsum, while
preserving some Unicode punctuation (e.g. ( and "), all Unicode marks (e.g. + and =) and control
characters (e.g. newline and tab), and replacing Unicode numbers with random digits between 0 and 9.

## License

Licensed under MIT license by [Tonic](https://www.tonic.ai).

## Requirements

Python 3.5+.

## Usage

Masking a file.

```
$ python mask.py <input_file.py>
```

Masking an input stream.

```
$ cat <input_file> | python mask.py
```

## Example

```
$ cat input.txt
Jane Little (DOB: 9-6-1977)

Jane Little seems to have had an inadequate response to treatment as yet. Symptoms of depression continue to be described. Her symptoms, as noted, are unchanged and they are just as frequent or intense as previously described. Jane Little describes feeling sad. Jane Little denies suicidal ideas or intentions. Jane Little reports the symptoms of this disorder continue unchanged. The subjective feeling of apprehension is occurring. Hypervigilance is occurring more frequently.

Participant(s) Developing the Plan:
- Susan Lobao (Counselor)
- Mary Golden (Client)

Diagnosis:
- Major depressive disorder, single episode, severe without psychotic features, F32.2 (ICD-10) (Active)
- Anxiety disorder, unspecified, F41.9 (ICD-10) (Active)

$ python mask.py input.txt
Lorem ipsum (dolor7-9-1525)

Integer ut nisi felis. Donec in tellus urna. Aenean ut condimentum nibh. In bibendum, tellus eget lacinia placerat, metus enim venenatis velit, a fringilla tellus ex eget justo. Cras quis vehicula eros. Nulla a posuere erat. Curabitur suscipit velit ac lectus venenatis, quis facilisis nulla tristique. Cras consequat gravida pharetra. Vestibulum consectetur massa quis leo finibus porttitor. Nullam maximus ipsum ligula, at imperdiet dui rutrum quis. Nunc nisl ex, hendrerit eu maximus n

Nullam luct(u)s lacus in risus bibe
-Mauris molest(ie elit p)
-Aliquam condi(mentum)

Nunc lacin
-Proin interdum sapien a accumsan mattis. Sed fringilla, elit eget rutrum viverra,49 1e(rat-06) (nisi s)
-Sed ultrices vehicula mollis. Null14a7 (mau-24)r(is vel)
```
