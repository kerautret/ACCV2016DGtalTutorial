SET(LIST3EXOS
     tuto3_curvature
  )

FOREACH(FILE ${LIST3EXOS})
  add_executable(${FILE} ${FILE})
  target_link_libraries (${FILE} ${DGTAL_LIBRARIES} ${TutoDependencies})
ENDFOREACH(FILE)

