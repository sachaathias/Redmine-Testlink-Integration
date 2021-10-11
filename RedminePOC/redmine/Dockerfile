FROM redmine
WORKDIR /usr/src/redmine
RUN git clone https://github.com/Byoskill/rp-testlinklink.git
RUN sed -i s/heads_for_wiki_formatter_without_testlinklink/super/g rp-testlinklink/lib/testlinklink_asset_tag_helper_patch.rb
RUN sed -i s/"alias_method_chain :heads_for_wiki_formatter, :testlinklink"//g rp-testlinklink/lib/testlinklink_asset_tag_helper_patch.rb
RUN mv rp-testlinklink ./plugins/redmine_testlinklink
