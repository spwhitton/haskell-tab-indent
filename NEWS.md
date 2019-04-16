0.2 (unreleased)
----------------

- Deactivate haskell-indentation-mode when activating
  haskell-tab-indent-mode.

  Recent haskell-mode considers haskell-indentation-mode to be the
  default, activating it unconditionally.  We follow
  haskell-indent-mode in deactivating it when activating our mode.

- Switch debian/changelog->NEWS.md.

0.1.0 (2015-12-05)
----------------

- Initial release.
