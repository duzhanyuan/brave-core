use_relative_paths = True

deps = {
  "vendor/ad-block": "https://github.com/brave/ad-block.git@67a8a19121f40d41e75468b2c26d6bace437ae4f",
  "vendor/tracking-protection": "https://github.com/brave/tracking-protection.git@bb6013ff4d0a0191ba93158f2f3b30e7fb18c5f6",
  "vendor/hashset-cpp": "https://github.com/brave/hashset-cpp.git@f86b0a5752545274e32c0dbb654c3592cc131c8a",
  "vendor/bloom-filter-cpp": "https://github.com/brave/bloom-filter-cpp.git@635780bbedff137a6a83ec23871944e22069de5b",
  "vendor/brave-extension": "https://github.com/brave/brave-extension.git@85aa24a86a9956bac37bba05c8c78b869a2f45f3",
  "vendor/requests": "https://github.com/kennethreitz/requests@e4d59bedfd3c7f4f254f4f5d036587bcd8152458",
  "vendor/boto": "https://github.com/boto/boto@f7574aa6cc2c819430c1f05e9a1a1a666ef8169b",
  "vendor/python-patch": "https://github.com/svn2github/python-patch@a336a458016ced89aba90dfc3f4c8222ae3b1403",
  "vendor/sparkle": "https://github.com/brave/Sparkle.git@c0759cce415d7c0feae45005c8a013b1898711f0",
  "vendor/bat-native-ledger": "https://github.com/brave-intl/bat-native-ledger@a3e64797bf6ebbfa39a60240db8d82995f97ebd9",
  "vendor/bat-native-rapidjson": "https://github.com/brave-intl/bat-native-rapidjson.git@86aafe2ef89835ae71c9ed7c2527e3bb3000930e",
  "vendor/bip39wally-core-native": "https://github.com/brave-intl/bip39wally-core-native.git@9b119931c702d55be994117eb505d56310720b1d",
  "vendor/bat-native-anonize": "https://github.com/brave-intl/bat-native-anonize.git@6f5817c5a4dcabb49e22b578ecae4993159e6481",
  "vendor/bat-native-tweetnacl": "https://github.com/brave-intl/bat-native-tweetnacl.git@05ed8f82faa03609fe5ae0a4c2d454afbe2ff267",
}

hooks = [
  {
    'name': 'bootstrap',
    'pattern': '.',
    'action': ['python', 'src/brave/script/bootstrap.py'],
  },
  {
    # Apply patches to chromium src
    'name': 'apply_patches',
    'pattern': '.',
    'action': ['python', 'src/brave/script/apply-patches.py'],
  },
  {
    # Run npm install for brave-extension
    'name': 'init',
    'pattern': '.',
    'action': ['python', 'src/brave/script/init-brave-extension.py'],
  }
]
