AM_LDFLAGS += -L$(top_builddir)/Hadrons
AM_CXXFLAGS += -I$(top_srcdir)

bin_PROGRAMS = \
  FlexibleContractor         \
  HadronsContractor          \
  HadronsNucContractor       \
  HadronsNucContractorMPI    \
  HadronsContractorCCMPI     \
  HadronsContractorBenchmark \
  HadronsXmlRun              \
  HadronsXmlValidate         \
  HadronsFermionEP64To32 

HadronsXmlRun_SOURCES = HadronsXmlRun.cpp
HadronsXmlRun_LDADD   = -lHadrons -lGrid

HadronsXmlValidate_SOURCES = HadronsXmlValidate.cpp
HadronsXmlValidate_LDADD   = -lHadrons -lGrid

HadronsFermionEP64To32_SOURCES  = EigenPackCast.cpp
HadronsFermionEP64To32_CXXFLAGS = $(AM_CXXFLAGS) -DFIN=WilsonImplD::FermionField -DFOUT=WilsonImplF::FermionField
HadronsFermionEP64To32_LDADD    = -lHadrons -lGrid

FlexibleContractor_SOURCES = FlexibleContractor.cpp
FlexibleContractor_LDADD   = -lHadrons -lGrid

HadronsContractor_SOURCES = Contractor.cpp
HadronsContractor_LDADD   = -lHadrons -lGrid

HadronsNucContractor_SOURCES = ContractorNuc.cpp
HadronsNucContractor_LDADD   = -lHadrons -lGrid

HadronsContractorCCMPI_SOURCES = ContractorCCMPI.cpp
HadronsContractorCCMPI_LDADD   = -lHadrons -lGrid

HadronsNucContractorMPI_SOURCES = ContractorNucMPI.cpp
HadronsNucContractorMPI_LDADD   = -lHadrons -lGrid

HadronsContractorBenchmark_SOURCES = ContractorBenchmark.cpp
HadronsContractorBenchmark_LDADD   = -lHadrons -lGrid
