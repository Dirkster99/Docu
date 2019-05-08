
This page contains a sequence of Layoutanchorable (tool window) drag \& drop test cases
(ranging from simple to complex) and their XML Layouts to better understand the relationships
between: [[LayoutAnchorablePaneGroup]], [[LayoutAnchorablePane]], and [[LayoutAnchorable]].

# Test Case 0
- Drag Tool 3 out of MainWindow

**Result**:
- LayoutAnchorablePaneGroup Orientation="Horizontal"
  - LayoutAnchorablePane\<Tool 3\>


## Test Case 1
- Drag Tool 3 out of MainWindow
- Drag Tool 2 into Dock.Bottom of Tool 3

**Result**:
- LayoutAnchorablePaneGroup Orientation="Vertical"
  - LayoutAnchorablePane\<Tool 3\>
  - LayoutAnchorablePane\<Tool 2\>


## Test Case 2
- Drag Tool 3 out of MainWindow
- Drag Tool 2 into Dock.Bottom of Tool 3
- Drag Tool 1 into Dock.Bottom of Tool 2

**Result**:
- LayoutAnchorablePaneGroup Orientation="Vertical"
  - LayoutAnchorablePane\<Tool 3\>
  - LayoutAnchorablePane\<Tool 2\>
  - LayoutAnchorablePane\<Tool 1\>


## Test Case 3
- Drag Tool 3 out of MainWindow
- Drag Tool 2 into Dock.Right of Tool 3

**Result**:
- LayoutAnchorablePaneGroup Orientation="Horizontal"
  - LayoutAnchorablePane\<Tool 3\>
  - LayoutAnchorablePane\<Tool 2\>


## Test Case 4
- Drag Tool 3 out of MainWindow
- Drag Tool 2 into Dock.Right of Tool 3
- Drag Tool 1 into Dock.Right of Tool 2

**Result**:
- LayoutAnchorablePaneGroup Orientation="Horizontal"
  - LayoutAnchorablePane\<Tool 3\>
  - LayoutAnchorablePane\<Tool 2\>
  - LayoutAnchorablePane\<Tool 1\>


## Test Case 5
- Drag Tool 3 out of MainWindow
- Drag Tool 2 into Dock.Center of Tool 3

**Result**:
- LayoutAnchorablePaneGroup Orientation="Horizontal"
  - LayoutAnchorablePane\<Tool 2\>, \<Tool 3\>


## Test Case 6
- Drag Tool 3 out of MainWindow
- Drag Tool 2 into Dock.Center of Tool 3
- Drag Tool 1 into Dock.Center of Tool 2

**Result**:
- LayoutAnchorablePaneGroup Orientation="Horizontal"
  - LayoutAnchorablePane\<Tool 1\>, \<Tool 2\>, \<Tool 3\>


## Test Case 7
- Drag Tool 3 out of MainWindow
- Drag Tool 2 into Dock.Right of Tool 3
- Drag Tool 1 into Dock.Bottom of Tool 2

**Result**:
- LayoutAnchorablePaneGroup Orientation="Horizontal"
  - LayoutAnchorablePane\<Tool 3\>
  - LayoutAnchorablePaneGroup Orientation="Vertical"
    - LayoutAnchorablePane\<Tool 2\>
    - LayoutAnchorablePaneGroup Orientation="Horizontal"
      - LayoutAnchorablePane\<Tool 1\>


## Test Case 8
- Drag Tool 3 out of MainWindow
- Drag Tool 2 into Dock.Bottom of Tool 3
- Drag Tool 1 into Dock.Right of Tool 2

**Result**:
- LayoutAnchorablePaneGroup Orientation="Vertical"
  - LayoutAnchorablePane\<Tool 3\>
  - LayoutAnchorablePaneGroup Orientation="Horizontal"
    - LayoutAnchorablePane\<Tool 2\>
    - LayoutAnchorablePaneGroup Orientation="Horizontal"
      - LayoutAnchorablePane\<Tool 1\>


# Test Case 9
- Drag Tool 3 out of MainWindow
- Drag Tool 2 into Dock.Right of Tool 3
- Drag Tool 1 into Dock.Bottom of Tool 2
- Drag FileStats into Dock.Bottom of Tool 3

**Result**:
- LayoutAnchorablePaneGroup Orientation="Horizontal"
  - LayoutAnchorablePaneGroup Orientation="Vertical"
    - LayoutAnchorablePane\<Tool 3\>
    - LayoutAnchorablePaneGroup Orientation="Horizontal"
      - LayoutAnchorablePane\<File Stats\>

  - LayoutAnchorablePaneGroup Orientation="Vertical"
    - LayoutAnchorablePane\<Tool 2\>
    - LayoutAnchorablePaneGroup Orientation="Horizontal"
      - LayoutAnchorablePane\<Tool 1\>
