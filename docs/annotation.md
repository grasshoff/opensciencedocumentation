
# annotation

Annotations can be created in different text formats of JSON, yaml, toml. These should be machine-readable and contain the annotation structure as json objects (lists of dictionaries).

### toml

The file format intends to create a simple UTF8 structured, easy to read text file for data entry.

- [TOML Definition](https://github.com/toml-lang/toml/blob/v0.5.0/README.md)

### yaml

The file format is a human readable file format equivalent to JSON data structures.

## slides

The annotation group *slides* is defined for presentation annotations to texts. Additional functions provide forward and backward presentation.

### keys and values

The associations and controls of the relationship between annotations, their text and the references to the annotation anchor (the text to which the annotation refers) and the presentation mode (the streamlit app with its containers), are done through specified key:value values.

### Example

``` yaml
slides:
    author : Gerd Graßhoff
    date: 5. Mai 2021
    title: Kausalität und Kausales Schliessen
    reference_scene: dict
    sl_pages:
      -
        sid : 0
        textid: kaus1
        pageid: 3
        annot : ```
          First slides in markdown. Additional markdown keys allow extensions such as bibliography, crossrefs and internal linking.
          ```

```
