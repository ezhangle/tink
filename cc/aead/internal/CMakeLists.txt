tink_module(aead::internal)

tink_cc_library(
  NAME cord_aes_gcm_boringssl
  SRCS
    cord_aes_gcm_boringssl.cc
    cord_aes_gcm_boringssl.h
  DEPS
    tink::subtle::random
    tink::subtle::subtle_util
    tink::subtle::subtle_util_boringssl
    tink::aead::cord_aead
    tink::util::errors
    tink::util::secret_data
    tink::util::status
    tink::util::statusor
    crypto
    absl::strings
    absl::cord
)
