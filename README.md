## Put Window


If you enable this extension the metacity move window keybindings are
replaced.

- - -

Changes:

__January 15, 2012__

 * added a config ui
 * position.x/y/width/height must be integers between 0 and 100 (was 0...1)

__December 17, 2011__

 * fix a bug that occures if the top panel is hidden.
  * checkout https://extensions.gnome.org/extension/42/auto-hide-top-panel/ it's awesome!

__December 11, 2011__

 * reduced the horizontal and vertical "gap" between windows
 * hitting move_to_center twice will now correctly maximize evolution

- - -

To check the predefined keyboard bindings (or modify them) open gconf-editor and
navigate to "apps.metacity.window_keybindings". (check the wiki for details)

* move_to_side_n.... move to north edge, height: 50% width 100%
* move_to_side_e.... move to easth edge, height: 100% width 50%
* move_to_side_s.... move to south edge, height: 50% width 100%
* move_to_side_w.... move to west  edge, height: 100% width 50%

* move_to_corners: widht 50% height 50%
* ne, se, sw, nw

* move_to_center.... move to center of the screen, widht 50% height 50%
                     Press twice to maximize the window

* move_to_workspace_1... resize to a configured location (see wiki for details)

Modify the keybindings using gconf-editor. The Treenode is
apps.metacity.window_keybindings.

- - -

**2 screen setup support**

  the extention works well with 2 screens in horizontal setup.

  Moving windows from one screen to another only possible widh side_e and side_w
  and only if windows was at side_e (or side_w) before. eg.

* a window in corner_nw of the right screen is not move to the left screen.
* a window at side_e of the right screen is move to the left screen (side_w)


- - -
### TODO

* 2 screens support vor vertical alignment
* a lot of things i currently dont remember :)


Check https://github.com/negesti/gnome-shell-extensions-negesti/tree/master/putWindow@clemens.lab21.org
for more details.
