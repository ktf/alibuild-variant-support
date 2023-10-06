# aliBuild variant support

This can be used to add variant support to aliBuild. 

A variant is an additional flag which is provided as part of the build package
in the form:

    <packagename>#<variant>

e.g. `O2Physics#tutorial`.

This can be used to specify that for a given package (O2Physics in this case),
the variable `ALIBUILD_BUILD_VARIANT` will be set while executing the recipe.

This allows customising builds depending on the variant. For the specific case,

    aliBuild build O2Physics#tutorial

will build only the tutorial part, not the whole O2Physics.

