0.3 (unreleased)
----------------

- When checking whether we're on the first line of where clause,
  require 'where' followed by end of line, rather than just a line
  starting with 'where'.

- Drop reference to an old git subtrees script from README.md.

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
