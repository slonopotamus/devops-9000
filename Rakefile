# frozen_string_literal: true

require 'asciidoctor'
require 'asciidoctor-revealjs'

task :convert do
  Asciidoctor.convert_file 'presentation.adoc', backend: 'revealjs'
end

task default: :convert
