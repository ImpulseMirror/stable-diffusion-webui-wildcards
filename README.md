# Wildcards with sorting
An extension version of a script from https://github.com/jtkelm2/stable-diffusion-webui-1/blob/main/scripts/wildcards.py

Allows you to use `__name__` syntax in your prompt to get a random line from a file named `name.txt` in the wildcards directory.

Allows you to sort generated images into folders based on a specified wildcard. 

When sort is enabled, `character` will look for the instances of `__character__` in a prompt and save images into the directory `/sorted/characters/{default_file_name #}.{extension}`
Providing an invalid wildcard will save to the default save path.

If rename is enabled, images will not duplicate into a `sorted` folder. Instead they will be renamed `{default_file_name #} character {character name}.{extension}`
