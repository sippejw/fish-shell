fish_svn_prompt - output svn information for use in a prompt
============================================================

Description
-----------


The fish_svn_prompt function can be used to display information about the current svn repository, if any.

For obvious reasons, it requires having svn installed.

There are numerous configuration options:


- $__fish_svn_prompt_color_revision, the colour of the revision number to display in the prompt
- $__fish_svn_prompt_char_separator, the separator between status characters

And
- $__fish_svn_prompt_char_added_display
- $__fish_svn_prompt_char_added_color

- $__fish_svn_prompt_char_conflicted_display
- $__fish_svn_prompt_char_conflicted_color

- $__fish_svn_prompt_char_deleted_display
- $__fish_svn_prompt_char_deleted_color

- $__fish_svn_prompt_char_ignored_display
- $__fish_svn_prompt_char_ignored_color

- $__fish_svn_prompt_char_modified_display
- $__fish_svn_prompt_char_modified_color

- $__fish_svn_prompt_char_replaced_display
- $__fish_svn_prompt_char_replaced_color

- $__fish_svn_prompt_char_unversioned_external_display
- $__fish_svn_prompt_char_unversioned_external_color

- $__fish_svn_prompt_char_unversioned_display
- $__fish_svn_prompt_char_unversioned_color

- $__fish_svn_prompt_char_missing_display
- $__fish_svn_prompt_char_missing_color

- $__fish_svn_prompt_char_versioned_obstructed_display
- $__fish_svn_prompt_char_versioned_obstructed_color

- $__fish_svn_prompt_char_locked_display
- $__fish_svn_prompt_char_locked_color

- $__fish_svn_prompt_char_scheduled_display
- $__fish_svn_prompt_char_scheduled_color

- $__fish_svn_prompt_char_switched_display
- $__fish_svn_prompt_char_switched_color

- $__fish_svn_prompt_char_token_present_display
- $__fish_svn_prompt_char_token_present_color

- $__fish_svn_prompt_char_token_other_display
- $__fish_svn_prompt_char_token_other_color

- $__fish_svn_prompt_char_token_stolen_display
- $__fish_svn_prompt_char_token_stolen_color

- $__fish_svn_prompt_char_token_broken_display
- $__fish_svn_prompt_char_token_broken_color

to choose the color and symbol for different parts of the prompt.

See also fish_vcs_prompt, which will call all supported vcs-prompt functions, including git, hg and svn.

Example
-------

A simple prompt that displays svn info::

    function fish_prompt
        ...
        printf '%s %s$' $PWD (fish_svn_prompt)
    end


