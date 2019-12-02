cmake_minimum_required(VERSION 2.8.4)

project(dispensa-mic NONE)

set(LATEX_COMPILER_FLAGS
  "--shell-escape"
  CACHE STRING "Flags passed to LaTeX")
include(UseLATEX.cmake)

add_latex_document(main.tex
  IMAGE_DIRS images)
add_latex_document(slide.tex
  IMAGE_DIRS images)
