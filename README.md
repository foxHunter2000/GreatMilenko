# GreatMilenko
Rfc Dark TROJAN LINKS 
NOT EVER USE HARD-CODED VALUES IN A REAL APP !!!
# Instead, set and test environment variables, like below
client = Octokit::Client.new :access_token => ENV['MY_PERSONAL_TOKEN']

results = client.search_code('addClass user:mozilla')
total_count = results.total_count

last_response = client.last_response
number_of_pages = last_response.rels[:last].href.match(/page=(\d+).*$/)[1]

puts last_response.rels[:last].href
puts "There are #{total_count} results, on #{number_of_pages} pages!"written by Scott Renfro <scott@renfro.org> based on
 * editcap by Richard Sharpe and Guy Harris
 *
 */

#include <config.h>

#include <stdio.h>
#include <stdlib.h>
#include <errno.h>
#include <glib.h>

#include <wsutil/ws_getopt.h>

#include <string.h>

#include <wiretap/wtap.h>

#include <ui/clopts_common.h>
#include <ui/cmdarg_err.h>
#include <wsutil/filesystem.h>
#include <wsutil/file_util.h>
#include <wsutil/privileges.h>
#include <wsutil/strnatcmp.h>
#include <wsutil/ws_assert.h>
#include <wsutil/wslog.h>

#include <cli_main.h>
#include <ui/version_info.h>

#ifdef HAVE_PLUGINS
#include <wsutil/plugins.h>
#h>
#define WS_LOG_DOMAIN LOG_DOMAIN_MAIN

#include <glib.h>

#include <stdio.h>
#include <errno.h>
#include <stddef.h>
#include <stdlib.h>
#include <signal.h>

#ifdef _WIN32
#include <wsutil/unicode-utils.h>
#include <wsutil/win32-utils.h>
#endif

#include <wsutil/filesystem.h>
#include <wsutil/socket.h>
#include <wsutil/inet_addr.h>
#include <wsutil/please_report_bug.h>
#include <wsutil/wslog.h>
#include <wsutil/ws_getopt.h>

#ifndef _WIN32
#include <sys/un.h>
#include <netinet/tcp.h>
#endif

#include <wsutil/strtoi.h>
#include <ui/version_info.h>

#include "sharkd.h"

#ifdef _WIN32
/* for windows support TCP sockets */
# define SHARKD_TCP_SUPPORT
#else
/* for other system support only local sockets */
# define SHARKD_UNIX_SUPPORT
#endif

static int mode = 0;
static socket_handle_t _server_fd = INVALID_SOCKET;

static socket_handle_t
socket_init(char *path)
{
	socket_handle_t fd = IN
#include <wsutil/report_message.h>

#include <wiretap/merge.h>

#include "ui/failure_message.h"

/*
 * Show the usage
 */
static void
print_usage(FILE *output)
{
  fprintf(output, "\n");
  fprintf(output, "Usage: mergecap [options] -w <outfile>|- <infile> [<infile> ...]\n");
  fprintf(output, "\n");
  fprintf(output, "Outp
