SET(REGISTRATION2_INCLUDES
../include/irtkImageAffineRegistration2.h
../include/irtkImageFreeFormRegistration2.h
../include/irtkImageRegistration2.h
../include/irtkImageRigidRegistration2.h
../include/irtkImageGradientFreeFormRegistration2.h
../include/irtkRegistration2.h
../include/irtkSparseFreeFormRegistration.h
../include/irtkTemporalImageRegistration.h
../include/irtkImageTFFDRegistration.h
../include/irtkImageTSFFDRegistration.h
)

SET(REGISTRATION2_SRCS 
irtkImageAffineRegistration2.cc
irtkImageFreeFormRegistration2.cc
irtkImageGradientFreeFormRegistration2.cc
irtkImageRegistration2.cc
irtkImageRigidRegistration2.cc
irtkSparseFreeFormRegistration.cc
irtkTemporalImageRegistration.cc
irtkImageTFFDRegistration.cc
irtkImageTSFFDRegistration.cc
)

ADD_LIBRARY(registration2++ ${REGISTRATION2_INCLUDES} ${REGISTRATION2_SRCS})

INSTALL_FILES(/include FILES ${REGISTRATION2_INCLUDES})
