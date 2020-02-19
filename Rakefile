# frozen_string_literal: true

require 'asciidoctor'
require 'asciidoctor-revealjs'

task :convert do
  Asciidoctor.convert_file 'presentation.adoc',
                           backend: 'revealjs',
                           safe: Asciidoctor::SafeMode::UNSAFE,
                           to_dir: 'build',
                           mkdirs: true
end

task default: :convert
