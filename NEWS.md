0.3 (unreleased)
----------------

- When checking for the first line of a where clause, require 'where'
  followed by end of line, rather than just a line starting with
  'where'.

- Recognise all declarations, not just top level declarations.  On
  lines following a declaration, always indent to the same level as
  the previous line, rather than indenting one further.

  Lines following declarations should either be indented to the same
  level as the declaration, or be blank.

- Always indent the first line of the contents of a where clause to
  one plus the level of the line containing 'where'.

  When doing so, try to fix the indentation of the line containing
  'where' if it's not correct.

- When one of the above cases does not apply, default to indenting to
  the same level of the previous line, unless the user explicitly
  invoked `indent-for-tab-command' (e.g. by hitting the tab key), in
  which case cycle between possible indents.

  This replaces treating the case where the current command is
  `newline-and-indent' specially.

- Reset indentation when current indentation is at least one more than
  the previous line, rather than just when it is exactly one more than
  the previous line.

  This should make it easier to unindent more than one line.

- Drop reference to an old git subtrees script from README.md.

- Code cleanup.

0.2 (2019-04-15)
----------------

- Deactivate haskell-indentation-mode when activating
  haskell-tab-indent-mode.

  Recent haskell-mode considers haskell-indentation-mode to be the
  default, activating it unconditionally.  We follow
  haskell-indent-mode in deactivating it when activating our mode.

- Switch debian/changelog->NEWS.md.

0.1.0 (2015-12-05)
------------------

- Initial release.
